# 📺 React TV Maze

A TV show search app built with React. Start typing a show name and results appear instantly with the show's poster, name and rating, using the free [TVMaze API](https://www.tvmaze.com/api).

## Features

- Live search as you type, debounced so the API isn't called on every keystroke
- Animated search box that expands with results (Framer Motion)
- Loading spinner while results are fetched, and a message when nothing is found
- Each result shows the poster, name and rating, and links to the show's TVMaze page
- Closes when you click outside it

## Tech stack

React 17 · styled-components · Framer Motion · Axios · React Icons · TVMaze REST API

## Run it locally

```bash
git clone https://github.com/Himu946/React-Tv-maze.git
cd React-Tv-maze
npm install
npm start
```

Then open http://localhost:3000.

## Project structure

```
src/
├── App.js                       # page layout
├── components/
│   ├── header/                  # logo header
│   ├── searchBar/               # search input, API call, results list
│   └── tvShow/                  # one search result
└── hooks/
    └── debounceHook.jsx         # custom useDebounce hook
```

## What I learned

- Building reusable React components with hooks (`useState`, `useEffect`, `useRef`)
- Writing a custom hook to debounce user input
- Fetching data from a REST API and handling loading and empty states
- Styling with styled-components and animating with Framer Motion
