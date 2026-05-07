# Портфолио проектов

## 1) warehouse-v2
Репозиторий: [fndpc/warehouse-v2](https://github.com/fndpc/warehouse-v2)  
Стек: `C#`, `.NET 8`, `WinForms`, `SQLite`

Запуск:
```powershell
git clone https://github.com/fndpc/warehouse-v2.git
cd warehouse-v2
dotnet restore WarehouseManager.slnx
dotnet run --project src/WarehouseManager.WinForms/WarehouseManager.WinForms.csproj
```

Использование: складской учет (товары, ячейки, приемка, перемещения, отгрузка, инвентаризация).

---

## 2) shortflow
Репозиторий: [whoaskeddd/shortflow](https://github.com/whoaskeddd/shortflow)  
Стек: `FastAPI`, `PostgreSQL`, `Redis`, `MinIO`, `React Native (Expo)`

Backend:
```powershell
git clone https://github.com/whoaskeddd/shortflow.git
cd shortflow
docker compose up --build
```

Frontend (mobile):
```powershell
cd apps/mobile
npm install
npx expo start
```

Использование: регистрация, лента, публикация видео, лайки, комментарии, поиск.

---

## 3) hrsystem-v2
Репозиторий: [whoaskeddd/hrsystem-v2](https://github.com/whoaskeddd/hrsystem-v2)  
Стек: `React + Vite + TypeScript` (frontend), `FastAPI` (backend)

Frontend:
```powershell
git clone https://github.com/whoaskeddd/hrsystem-v2.git
cd hrsystem-v2/frontend
npm install
npm run dev
```

Backend:
```powershell
cd ..
docker compose up --build
```

Использование: интерфейс HR-платформы (вакансии/резюме/отклики/чат).

---

## 4) warehouse-ai-accounting
Репозиторий: [whoaskeddd/warehouse-ai-accounting](https://github.com/whoaskeddd/warehouse-ai-accounting)

Запуск: в текущем репозитории нет frontend/backend для запуска.

Использование: спецификация системы складского учета с AI-прогнозированием.

---

## 5) thebestmessenger
Репозиторий: [whoaskeddd/thebestmessenger](https://github.com/whoaskeddd/thebestmessenger)  
Стек: `FastAPI`

Backend:
```powershell
git clone https://github.com/whoaskeddd/thebestmessenger.git
cd thebestmessenger/backend
python -m venv .venv
.venv\Scripts\activate
pip install fastapi uvicorn
uvicorn app.main:app --reload
```

Frontend: отсутствует в репозитории.

Использование: базовый API-сервер, проверка через `http://127.0.0.1:8000/`.
