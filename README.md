# JobPop Frontend

Frontend приложение для JobPop - платформы поиска временной работы.

## 🚀 Технологии

- **Next.js 15** - React фреймворк
- **TypeScript** - Типизация
- **Tailwind CSS** - Стилизация
- **Radix UI** - UI компоненты
- **React Hook Form + Zod** - Формы и валидация
- **React Context** - Управление состоянием

## 📦 Установка

```bash
npm install
```

## 🏃‍♂️ Запуск

```bash
# Разработка
npm run dev

# Продакшн
npm run build
npm start
```

## 🌐 Переменные окружения

Создайте файл `.env.local`:

```env
NEXT_PUBLIC_API_URL=http://localhost:3001/api
```

## 🚀 Деплой

### Vercel (Рекомендуется)
1. Подключите репозиторий к Vercel
2. Установите переменную: `NEXT_PUBLIC_API_URL=https://your-backend-url.com/api`
3. Деплой автоматический

### Netlify
1. Подключите репозиторий к Netlify
2. Build command: `npm run build`
3. Publish directory: `.next`
4. Установите переменную окружения

## 📱 Функции

- ✅ Поиск вакансий с фильтрами
- ✅ Размещение вакансий (для работодателей)
- ✅ Аутентификация пользователей
- ✅ Переключение языков (RU/EN)
- ✅ Адаптивный дизайн
- ✅ Real-time обновления

## 🔗 Связанные репозитории

- **Backend**: [jobpop-backend](../jobpop-backend)
- **Полный проект**: [JobPop-main](../JobPop-main)

---

**JobPop** - Connecting people with opportunities! 🚀