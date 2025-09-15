# JobPop - Быстрый старт

## 🚀 Запуск за 5 минут

### Вариант 1: Docker (Рекомендуется)

```bash
# Клонируйте репозиторий
git clone <repository-url>
cd JobPop-main

# Запустите приложение
./start.sh
```

Приложение будет доступно по адресам:
- **Frontend**: http://localhost:3000
- **Backend API**: http://localhost:5000
- **MongoDB**: mongodb://admin:password@localhost:27017/jobpop

### Вариант 2: Локальная установка

#### 1. Backend

```bash
cd backend
npm install
cp env.example .env
# Отредактируйте .env файл
npm start
```

#### 2. Frontend

```bash
cd jobpop
npm install
# Создайте .env.local с NEXT_PUBLIC_API_URL=http://localhost:5000/api
npm run dev
```

## 🎯 Основные функции

### Для работников:
- ✅ Поиск вакансий с фильтрами
- ✅ Подача заявок на работы
- ✅ Просмотр профиля и статистики
- ✅ Переключение языков (RU/EN)

### Для работодателей:
- ✅ Размещение вакансий
- ✅ Просмотр заявок
- ✅ Управление вакансиями
- ✅ Переключение языков (RU/EN)

## 🔧 Настройка

### Backend (.env)
```env
PORT=5000
NODE_ENV=development
MONGODB_URI=mongodb://localhost:27017/jobpop
JWT_SECRET=your-super-secret-jwt-key-here
JWT_EXPIRE=7d
CORS_ORIGIN=http://localhost:3000
```

### Frontend (.env.local)
```env
NEXT_PUBLIC_API_URL=http://localhost:5000/api
```

## 📱 Тестирование

1. Откройте http://localhost:3000
2. Зарегистрируйтесь как работник или работодатель
3. Попробуйте разместить вакансию (для работодателей)
4. Попробуйте найти вакансии (для работников)
5. Переключите язык в правом верхнем углу

## 🐛 Устранение неполадок

### Порт занят
```bash
# Остановите все контейнеры
docker-compose down

# Или измените порты в docker-compose.yml
```

### MongoDB не подключается
```bash
# Проверьте статус контейнеров
docker-compose ps

# Посмотрите логи
docker-compose logs mongodb
```

### Frontend не загружается
```bash
# Проверьте переменные окружения
cat jobpop/.env.local

# Пересоберите контейнер
docker-compose up --build frontend
```

## 📚 Дополнительная информация

- [Полное руководство по развертыванию](DEPLOYMENT.md)
- [API документация](backend/README.md)
- [Frontend документация](jobpop/README.md)

## 🆘 Поддержка

Если у вас возникли проблемы:
1. Проверьте логи: `docker-compose logs -f`
2. Убедитесь, что все порты свободны
3. Проверьте настройки .env файлов
4. Создайте issue в репозитории
