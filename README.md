# MClient

**Веб-клиент для почтового сервиса на базе React, TypeScript и Vite.**

## Ссылка для преподавателя для проверки работы
```bash
31.128.51.50:5173/login
```

## 📎 Описание

MClient позволяет пользователям:
- Регистрироваться и входить в систему
- Отправлять, получать и просматривать сообщения
- Управлять списком отправленных и полученных сообщений

Клиент взаимодействует с REST API сервера через Axios.

## 🛠 Технологии

- React 18
- TypeScript
- Vite (с HMR)
- Redux Toolkit
- Axios
- ESLint + Prettier
- Docker и Docker Compose (опционально)

## 🚀 Быстрый старт

### 1. Клонировать репозиторий
```bash
git clone <repository-url> mclient
cd mclient
```

### 2. Установить зависимости
```bash
npm install
```

### 3. Запустить приложение

#### Локально
```bash
npm run dev
```
Откройте http://localhost:5173 в браузере.

#### В Docker (опционально)
```bash
docker-compose up --build
```
Сервис будет доступен по тому же адресу.

## ⚙️ Переменные окружения

В файл `.env` (или через переменные окружения Docker) можно задать:
```
VITE_API_URL=http://host.docker.internal:8080/api/v1
```

## 🔧 Скрипты

- `npm run dev` — запуск dev сервера
- `npm run build` — сборка production
- `npm run preview` — предпросмотр production сборки

## 📁 Структура проекта

```
src/
├── api/        Настройка HTTP-клиента
├── app/        Redux store и хуки
├── components/ Переиспользуемые UI-компоненты
├── features/   Логика приложения (Redux slices)
└── pages/      Маршрутизируемые страницы
```
