# MedTracker

**MedTracker** is a full‑stack MERN‑style application implemented in TypeScript. It helps users track medication and prescription data while providing AI-powered chat features and secure authentication. The project pairs a React/Vite frontend with a Node/Express backend and is container‑ready via Docker.

---

## 🚀 Key Features

- **Modern frontend** using React and Vite for fast development and hot-reloading
- **TypeScript throughout** for strong typing on both client and server
- **User authentication** with state management (`authStore.ts`)
- **AI/chat integrations** (`chatService.ts`, `geminiService.ts`) for enhanced user interactions
- **Backend API** served from `server.ts`, suitable for MongoDB or other data storage
- **Dockerized setup** via `Dockerfile` and `docker-compose.yml` for easy deployment
- **Sample data** in `fake_prescription_test/` for testing or demonstration

---

## 🗂️ Project Structure

```text
MedTracker/
├── Dockerfile
├── docker-compose.yml
├── .env.example          # environment variables template
├── index.html            # entry point for the frontend
├── server.ts             # Express server startup
├── package.json          # dependencies & scripts
├── tsconfig.json
├── vite.config.ts        # Vite configuration
├── src/
│   ├── App.tsx           # root React component
│   ├── main.tsx          # ReactDOM render + providers
│   ├── index.css         # global styles
│   ├── services/         # external service clients
│   │   ├── chatService.ts
│   │   └── geminiService.ts
│   └── store/
│       └── authStore.ts  # opensignin/signup state
└── fake_prescription_test/  # sample prescription images
```

> The repository is configured for both local development and containerized environments.

---

## 🛠️ Getting Started

### Prerequisites

- Node.js **18+**
- npm (or yarn)
- Docker & Docker Compose (optional but recommended)

### Installation

```bash
# clone the repository
git clone <repo-url>
cd MedTracker

# install packages
npm install  # or yarn install
```

### Running Locally

```bash
npm run dev
```

This starts the Vite dev server for the frontend. If the backend API is used, run:

```bash
npm run start
# or directly
# ts-node server.ts
```

### Building for Production

```bash
npm run build
```

### Docker Usage

```bash
docker-compose up --build
```

This command builds both frontend and backend images and starts the stack.

---

## 📦 Scripts

| Script           | Description                        |
|------------------|------------------------------------|
| `npm run dev`    | Start frontend development server  |
| `npm run build`  | Build production bundle            |
| `npm run start`  | Launch backend server              |
| `docker-compose` | Build and run containers           |

---

## 📝 Notes

- See `.env.example` for required environment variables.
- Customize services or add a MongoDB connection in `server.ts`.
- The `fake_prescription_test` folder contains example images used for testing or UI previews.

---

## 🧩 Contributions

Contributions are welcome! Feel free to open issues or submit pull requests.

---

*Thank you for checking out MedTracker!*




