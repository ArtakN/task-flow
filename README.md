
# Task Flow

Task Flow is a Kanban-style task management web application for organizing tasks across multiple boards and lists.

Developed as a personal portfolio project using React, TypeScript, Zustand, and Feature-Sliced Design (FSD).

## 🌐 Live Demo

[Open Task Flow](https://task-flow-6c09a.web.app/)

[Developer Portfolio](https://artaknavoyan.xyz)

## ✨ Features

### Board Management
- Create, edit, and delete boards.
- Default lists: To Do, In Progress, and Done.
- Cascading deletion of associated lists and tasks.

### List Management
- Create, edit, and delete lists.
- Dynamic rendering of lists within selected boards.

### Task Management
- Create, edit, and delete task cards.
- Drag and drop tasks between lists.
- Inline text editing.
- Confirmation dialogs for destructive actions.

### Data Persistence
- Browser localStorage persistence using Zustand middleware.
- Automatic state restoration after page reload.

### User Interface
- Responsive interface.
- Context menus using Shadcn UI and Radix UI.
- Auto-resizing text areas.
- Component-based architecture.

## 🛠️ Tech Stack

| Technology | Purpose |
|---|---|
| React 19 | User interface |
| TypeScript | Type safety |
| Vite | Development and build tooling |
| Zustand | State management |
| Tailwind CSS v4 | Styling |
| React Router | Client-side routing |
| Shadcn UI / Radix UI | UI components |
| Lucide React | Icons |
| Firebase Hosting | Deployment |
| ESLint / Prettier | Code quality |

## 🏗️ Architecture

The project follows Feature-Sliced Design (FSD), separating application logic into dedicated layers:

- `app` — application initialization and configuration.
- `pages` — application pages.
- `widgets` — independent UI sections.
- `features` — user-facing functionality.
- `entities` — board, list, and task entities.
- `shared` — reusable components and utilities.

State management is organized into separate Zustand stores for boards, lists, and tasks, using optimized selectors and persistence middleware.

Public slice APIs provide explicit boundaries between modules.

## 🚀 Getting Started

### 1. Clone the repository

```bash
git clone https://github.com/ArtakN/task-flow.git
cd task-flow
```

### 2. Install dependencies

```bash
npm install
```

### 3. Environment configuration (optional)

If Firebase configuration is required, create a `.env.local` file with the relevant environment variables.

```env
VITE_FIREBASE_API_KEY=your_key
VITE_FIREBASE_AUTH_DOMAIN=your_auth_domain
```

### 4. Start the development server

```bash
npm run dev
```

Open http://localhost:5173 in your browser, or use the URL displayed in the terminal.

## 📜 Available Scripts

| Command | Description |
|---|---|
| `npm run dev` | Start development server |
| `npm run build` | Create production build |
| `npm run lint` | Run ESLint |
| `npm run lint:fix` | Fix supported linting issues |
| `npm run preview` | Preview production build |

## 📦 Deployment

The application is deployed using Firebase Hosting.

[Live Application](https://task-flow-6c09a.web.app/)

The current deployed version uses localStorage for data persistence.

## 🎯 Planned Improvements

- Unit and integration tests with Vitest and React Testing Library.
- Firebase Authentication.
- Firestore integration and cloud persistence.
- Improved loading states and error handling.
- Task descriptions, labels, and due dates.
- Search and filtering.

## 👨‍💻 Author

Artak Navoyan — Frontend Developer

- [Portfolio](https://artaknavoyan.xyz)
- [GitHub](https://github.com/ArtakN)
- [LinkedIn](https://www.linkedin.com/in/artaknavoyan/)
- [Email](mailto:navoyan.ab@gmail.com)
