# 🚀 Деплой Frontend (JobPop)

## Варианты деплоя

### 1. Vercel (Рекомендуется)

**Преимущества:**
- ✅ Создан командой Next.js
- ✅ Автоматический деплой из GitHub
- ✅ Бесплатный план
- ✅ Автоматические SSL сертификаты
- ✅ CDN по всему миру

**Шаги:**
1. Зайдите на [vercel.com](https://vercel.com)
2. Войдите через GitHub
3. Нажмите "New Project"
4. Выберите репозиторий `jobpop-frontend`
5. Настройте переменные окружения:
   ```
   NEXT_PUBLIC_API_URL=https://your-backend-url.com/api
   ```
6. Нажмите "Deploy"

### 2. Netlify

**Шаги:**
1. Зайдите на [netlify.com](https://netlify.com)
2. Подключите GitHub репозиторий
3. Настройте:
   - Build command: `npm run build`
   - Publish directory: `.next`
4. Добавьте переменную окружения:
   ```
   NEXT_PUBLIC_API_URL=https://your-backend-url.com/api
   ```

**Примечание:** Файл `netlify.toml` уже настроен в проекте для автоматической конфигурации.

### 3. Railway

**Шаги:**
1. Зайдите на [railway.app](https://railway.app)
2. Подключите GitHub репозиторий
3. Выберите папку `jobpop-frontend`
4. Добавьте переменную окружения
5. Деплой автоматический

## 🔧 Настройка переменных окружения

Для продакшна установите:
```
NEXT_PUBLIC_API_URL=https://your-backend-domain.com/api
```

## 📱 Проверка после деплоя

1. Откройте ваш сайт
2. Проверьте регистрацию/вход
3. Проверьте поиск вакансий
4. Проверьте переключение языков
5. Проверьте размещение вакансий (для работодателей)

## 🔗 Связанные проекты

- **Backend**: [jobpop-backend](../jobpop-backend)
- **Полный проект**: [JobPop-main](../JobPop-main)
