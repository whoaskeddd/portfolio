# Портфолио проектов

Единый репозиторий-витрина моих работ с краткими инструкциями по запуску и использованию.

## 1) warehouse-v2

Репозиторий: [fndpc/warehouse-v2](https://github.com/fndpc/warehouse-v2)  
Стек: `C#`, `.NET 8`, `WinForms`, `SQLite`

### Кратко
Desktop-приложение для складского учета: справочники, приемка, перемещения, отгрузка, инвентаризация, аудит.

### Запуск
```powershell
git clone https://github.com/fndpc/warehouse-v2.git
cd warehouse-v2
dotnet restore WarehouseManager.slnx
dotnet build src/WarehouseManager.WinForms/WarehouseManager.WinForms.csproj
dotnet run --project src/WarehouseManager.WinForms/WarehouseManager.WinForms.csproj
```

### Использование
1. Вкладка `Справочники`: создать товары и ячейки.
2. Вкладка `Операции`: сделать первую приемку.
3. Вкладки `Остатки` и `Инвентаризация`: проверить остатки и расхождения.

---

## 2) shortflow

Репозиторий: [whoaskeddd/shortflow](https://github.com/whoaskeddd/shortflow)  
Стек: `React Native (Expo)`, `FastAPI`, `PostgreSQL`, `Redis`, `MinIO`, `Docker`

### Кратко
Mobile-first MVP коротких видео (лента, лайки, комментарии, публикация, базовая AI-модерация).

### Запуск
```powershell
git clone https://github.com/whoaskeddd/shortflow.git
cd shortflow
docker compose up --build
```

Отдельно мобильный клиент:
```powershell
cd apps/mobile
npm install
npx expo start
```

### Использование
1. Проверить backend: `http://127.0.0.1:8000/health`.
2. Запустить Android Emulator и открыть приложение через Expo (`a` в терминале).
3. Пройти сценарий: регистрация -> лента -> публикация видео -> комментарии/лайки.

---

## 3) hrsystem-v2

Репозиторий: [whoaskeddd/hrsystem-v2](https://github.com/whoaskeddd/hrsystem-v2)  
Стек: `React + Vite + TypeScript + Tailwind`, backend `FastAPI` (пока каркас)

### Кратко
HR-платформа в стиле hh.ru (вакансии, резюме, отклики, чат, роли). Сейчас репозиторий в стадии активной подготовки.

### Запуск
Фронтенд:
```powershell
git clone https://github.com/whoaskeddd/hrsystem-v2.git
cd hrsystem-v2/frontend
npm install
npm run dev
```

Через Docker Compose (frontend + backend placeholder):
```powershell
cd ..
docker compose up --build
```

### Использование
1. Открыть frontend по адресу `http://localhost:5173`.
2. Проверять UI-сценарии и навигацию.
3. Для API ориентироваться на `docs/api/openapi.json` до полной реализации backend.

---

## 4) warehouse-ai-accounting

Репозиторий: [whoaskeddd/warehouse-ai-accounting](https://github.com/whoaskeddd/warehouse-ai-accounting)  
Статус: в текущем виде это в основном ТЗ/план (`README.md`, `plan.md`)

### Кратко
Концепт desktop-системы складского учета с AI-прогнозированием спроса и рекомендациями закупок.

### Запуск
На текущем этапе запускаемого приложения в репозитории нет.

### Использование
1. Использовать как проектную спецификацию.
2. На основе `README.md` и `plan.md` реализовывать MVP (модули, БД, AI-часть, UI).

---

## 5) thebestmessenger

Репозиторий: [whoaskeddd/thebestmessenger](https://github.com/whoaskeddd/thebestmessenger)  
Стек: `FastAPI` (backend-черновик)

### Кратко
Проект мессенджера; в backend есть минимальный FastAPI-сервер с тестовым endpoint.

### Запуск
```powershell
git clone https://github.com/whoaskeddd/thebestmessenger.git
cd thebestmessenger/backend
python -m venv .venv
.venv\Scripts\activate
pip install fastapi uvicorn
uvicorn app.main:app --reload
```

### Использование
1. Открыть `http://127.0.0.1:8000/`.
2. Проверить ответ `hello!`.
3. Далее наращивать API-модули по `docs/` и `plan.md`.

---

## Видео-демо (добавлю позже)

Папка для роликов уже подготовлена:

```text
assets/videos/
```

План по именам файлов:

```text
warehouse-v2.mp4
shortflow.mp4
hrsystem-v2.mp4
warehouse-ai-accounting.mp4
thebestmessenger.mp4
```
