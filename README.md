# MedTracker

MedTracker is a TypeScript-based web application for managing medical information and prescriptions. It utilizes modern tooling including Vite, React, and server-side APIs to provide a responsive user interface.

## Features

- Authentication and user state management (via `authStore`)
- Chat and Gemini services for communication (`chatService.ts`, `geminiService.ts`)
- Responsive React application built with Vite
- Docker support via `Dockerfile` and `docker-compose.yml`

## Project Structure

```
├── Dockerfile
├── docker-compose.yml
├── index.html
├── package.json
├── server.ts             # Express or custom server entrypoint
├── tsconfig.json
├── vite.config.ts
├── src/
│   ├── App.tsx
│   ├── main.tsx
│   ├── index.css
│   ├── services/
│   │   ├── chatService.ts
│   │   └── geminiService.ts
│   └── store/
│       └── authStore.ts
└── fake_prescription_test/  # test directory or simulation data
```

## Getting Started

### Prerequisites

- Node.js (>=18 recommended)
- npm or yarn
- Docker (optional, for containerized setup)

### Installation

```bash
# clone the repo
git clone <repo-url>
cd MedTracker

# install dependencies
npm install
# or
# yarn install
```

### Development

To start the development server:

```bash
npm run dev
```

This will launch the Vite development server and open the app in your default browser. The server backend (if any) may run via `npm run start` or using the `server.ts` entrypoint.

### Building for Production

```bash
npm run build
```

### Docker

Build and run using Docker Compose:

```bash
docker-compose up --build
```





