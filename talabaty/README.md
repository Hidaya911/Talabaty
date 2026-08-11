# Talabaty Project


## Structure

```
talabaty-merged/
├── backend/     Express + TypeScript + MongoDB API
├── frontend/    React + TypeScript + Vite app
└── archive/     Original files that weren't safe to wire into the live app (see below)
```

## Running it

**Backend**
```bash
cd backend
npm install
cp .env.example .env      # fill in MONGO_URI / JWT_SECRET
npm run dev                # http://localhost:5000
```

**Frontend**
```bash
cd frontend
npm install
cp .env.example .env      # defaults to http://localhost:5000/api
npm run dev                 # http://localhost:5173
```

`npm run build` runs `tsc` first on both, so a failing type check fails the build — that's your
zero-errors guardrail going forward too.

