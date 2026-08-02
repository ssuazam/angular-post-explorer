# Angular Post Explorer

Angular application for exploring posts from the JSONPlaceholder public API.
It demonstrates reactive search, filtering, sorting, loading states, error
handling, and a responsive TailwindCSS interface.

## Features

- Fetches posts from `https://jsonplaceholder.typicode.com/posts`.
- Reactive title search with RxJS debounce.
- User ID filtering.
- Sort by title, ID, or user ID.
- Reusable custom order pipe.
- Loading and error states.
- Detail modal for each post.
- Responsive UI with TailwindCSS.

## Tech Stack

- Angular 20
- TypeScript
- RxJS
- TailwindCSS
- JSONPlaceholder API

## Project Structure

```text
src/
├── app/
│   ├── components/
│   │   └── post-list.component.*
│   ├── pipes/
│   │   └── order-by-pipe.ts
│   └── services/
│       └── post.service.ts
└── styles.scss
```

## Run Locally

```bash
npm install
npm start
```

Open `http://localhost:4200`.

## Build

```bash
npm run build
```

## Portfolio Notes

This project is a compact frontend example focused on Angular data flow:

- `BehaviorSubject` models UI inputs.
- `combineLatest` joins search and filter state.
- `switchMap` cancels stale requests.
- A custom pipe handles client-side ordering.

Recommended GitHub repository name: `angular-post-explorer`.

## Author

Santiago Suaza
