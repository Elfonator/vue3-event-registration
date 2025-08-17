# Event Registration (Vue 3)

Small learning project: an event booking app built with Vue 3 (Composition API).
It showcases optimistic UI, error handling with retry, and shared state via a composable.

## Features

- Optimistic booking (pending → confirmed) with rollback on failure
- Duplicate-registration guard per user/event
- `useBookings()` composable to share state/actions
- Empty and error states + “Retry” action
- Responsive UI with Tailwind; Lucide icons (dynamic spinner/check)

## Tech

Vue 3 + Vite, Composition API, Tailwind CSS, lucide-vue-next, Fetch API.

## Getting started

1. **Install**

```bash
npm install
```

2. **Mock API (JSON server)**

```bash
npm install --save-dev json-server
npx json-server --watch db.json --port 3001
# Example db.json:
# {
#   "events": [     {
#     "id": "2",
#     "title": "Vue Conference 2024",
#     "date": "2024-05-20",
#     "description": "Join us for a day of insightful talks and networking with industry leaders in technology.",
#     "location": "Convention Center, Downtown"
#    }],
#   "bookings": []
# }
```

3. **\*Run the app**

```bash
npm run dev
```
