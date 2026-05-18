# Task Manager

Modern task management application built with React, Vite, and Tailwind CSS, focused on clean architecture, accessibility, and a polished user experience.

## Tech Stack

- **React 19** — functional components, hooks, Context API, and routing with React Router v7
- **Tailwind CSS v4** — utility-first styling with a custom dark theme
- **Vite** — fast bundling and development environment
- **Motion** — animation library for smooth task transitions and reordering
- **uuid** — unique task ID generation
- **tailwind-merge** — conflict-safe Tailwind class merging
- **lucide-react** — scalable and customizable icon library

## Features

- Create tasks with title, description, and due date
- Inline task editing directly from the list
- Filter tasks by All, Pending, or Completed
- Dynamic expiration badges for upcoming and overdue tasks
- Form validation with clear and immediate feedback
- Keyboard-friendly interactions
  - `Enter` submits forms
  - `Shift + Enter` adds line breaks inside descriptions
- Mark tasks as completed with automatic list reordering
- Inline delete confirmation flow
- Dedicated task details page
- Real-time completed task counter
- Persistent task storage using `localStorage`
- Smooth animated list transitions
- Illustrated empty state for improved user experience

## Project Structure

```txt
src/
  contexts/       # TasksContext and TasksProvider
  hooks/          # useTasks, useTasksContext and related tests
  constants/      # storage and filter constants
  components/     # reusable UI components
  pages/          # HomePage and TaskPage
  test/           # global test setup
```

## Getting Started

```bash
npm install
npm run dev
```

## Testing

Tests are colocated with their respective modules (e.g. `useTasks.test.js` alongside `useTasks.js`) using Vitest and Testing Library.

```bash
npm test          # watch mode
npm run coverage  # coverage report
```
