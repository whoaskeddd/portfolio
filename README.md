# Portfolio

Сборник моих проектов в `C:\develop\portfolio\repos`.

## Проекты

### 1. HRSystem v2
- Репозиторий: [whoaskeddd/hrsystem-v2](https://github.com/whoaskeddd/hrsystem-v2)
- Стек: `React`, `Vite`, `TypeScript` (frontend), backend пока placeholder
- Демо-видео: [HRSYSTEM.mp4](https://github.com/whoaskeddd/portfolio/blob/main/assets/videos/HRSYSTEM.mp4)

Запуск frontend:
```powershell
cd C:\develop\portfolio\repos\hrsystem-v2\frontend
npm install
npm run dev
```

Запуск через Docker Compose:
```powershell
cd C:\develop\portfolio\repos\hrsystem-v2
docker compose up --build
```

Использование: UI HR-платформы (landing, вакансии, резюме, сообщения, звонки, админка).

---

### 2. ShortFlow
- Репозиторий: [whoaskeddd/shortflow](https://github.com/whoaskeddd/shortflow)
- Стек: `FastAPI`, `PostgreSQL`, `Redis`, `MinIO`, `React Native (Expo)`
- Демо-видео: [shortflowfull.mp4](https://github.com/whoaskeddd/portfolio/blob/main/assets/videos/shortflowfull.mp4)

Запуск backend + инфраструктуры:
```powershell
cd C:\develop\portfolio\repos\shortflow
docker compose up --build
```

Запуск frontend (mobile):
```powershell
cd C:\develop\portfolio\repos\shortflow\apps\mobile
npm install
npx expo start
```

Использование: регистрация, лента, публикация видео, лайки, комментарии, поиск, уведомления.

---

### 3. TheBestMessenger
- Репозиторий: [whoaskeddd/thebestmessenger](https://github.com/whoaskeddd/thebestmessenger)
- Стек: `FastAPI` (минимальный backend)
- Демо-видео: [thebestmessenger.mp4](https://github.com/whoaskeddd/portfolio/blob/main/assets/videos/thebestmessenger.mp4)

Запуск backend:
```powershell
cd C:\develop\portfolio\repos\thebestmessenger\backend
uv sync
uv run uvicorn app.main:app --host 0.0.0.0 --port 8000 --reload
```

Проверка:
- `http://127.0.0.1:8000/` -> `"hello!"`

Frontend: пока отсутствует в репозитории.

---

### 4. Warehouse AI Accounting
- Репозиторий: [whoaskeddd/warehouse-ai-accounting](https://github.com/whoaskeddd/warehouse-ai-accounting)
- Формат: спецификация и план проекта
- Демо-видео: [WAREHOUSEAI.mp4](https://github.com/whoaskeddd/portfolio/blob/main/assets/videos/WAREHOUSEAI.mp4)
```powershell
Запуск
dotnet restore SmartStockAI.sln
dotnet build SmartStockAI.sln
dotnet run --project .\src\SmartStockAI.App\SmartStockAI.App.csproj
dotnet run --project src/WarehouseManager.WinForms/WarehouseManager.WinForms.csproj
```
---

### 5. Warehouse Manager v2
- Репозиторий: [fndpc/warehouse-v2](https://github.com/fndpc/warehouse-v2)
- Стек: `C#`, `.NET 8`, `WinForms`, `SQLite`
- Демо-видео: [warehousev2.mp4](https://github.com/whoaskeddd/portfolio/blob/main/assets/videos/warehousev2.mp4)

Запуск:
```powershell
cd C:\develop\portfolio\repos\warehouse-v2
dotnet restore WarehouseManager.slnx
dotnet build src/WarehouseManager.WinForms/WarehouseManager.WinForms.csproj
dotnet run --project src/WarehouseManager.WinForms/WarehouseManager.WinForms.csproj
```

Использование: справочники, приемка, перемещения, отгрузка, остатки, инвентаризация, аудит.

---

## Примечание по структуре
`portfolio` — это родительский репозиторий с подключенными submodule (`repos/*`).
Изменения в каждом проекте коммитятся внутри соответствующего submodule, после этого нужно коммитить обновленные ссылки submodule в `portfolio`.


