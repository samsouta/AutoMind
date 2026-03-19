Telegram (User Account)
        ↓
   Telethon Client
        ↓
   Message Ingestor
        ↓
   Redis Queue (buffer)
        ↓
   Worker Pool (async)
        ↓
 ┌───────────────┬───────────────┬───────────────┐
 │ AI Processor  │ Rule Engine   │ Parser Engine │
 └───────────────┴───────────────┴───────────────┘
        ↓
   Action Engine
        ↓
 ┌───────────────┬───────────────┬───────────────┐
 │ Reminder      │ Summary       │ Forwarding    │
 │ Task Creator  │ Notification  │ Storage       │
 └───────────────┴───────────────┴───────────────┘
        ↓
 PostgreSQL (data)
        ↓
 API Layer (FastAPI)
        ↓
 Frontend Dashboard (React)