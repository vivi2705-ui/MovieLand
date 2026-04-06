# MovieLand

A React application that lets you search for movies using the [OMDb API](http://www.omdbapi.com/).

---

## Preview

> Search for any movie and instantly see results with posters, release years, and types.

---

## Features

- Search movies by title in real time
- Displays movie poster, title, year, and type
- Fallback image for movies with no poster
- Clean and responsive UI

---

## Tech Stack

- [React](https://reactjs.org/) — UI library
- [OMDb API](http://www.omdbapi.com/) — Movie data source
- CSS — Custom styling

---

## Getting Started

### Prerequisites

Make sure you have **Node.js** and **npm** installed.

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/your-username/movieland.git

# 2. Navigate into the project
cd movieland

# 3. Install dependencies
npm install

# 4. Start the development server
npm start
```

The app will run at `http://localhost:3000`.

---

## API Key

This project uses the [OMDb API](http://www.omdbapi.com/apikey.aspx). The key is already included for demo purposes. To use your own:

1. Register for a free key at [omdbapi.com](http://www.omdbapi.com/apikey.aspx)
2. Replace the key in `App.js`:

```js
const API_URL = "http://www.omdbapi.com?apikey=YOUR_KEY_HERE";
```

---

---

## How It Works

1. On load, the app fetches movies by default via `useEffect`.
2. The `searchMovies` function calls the OMDb API with the given title.
3. Results are stored in React state and passed to `MovieCard` components for rendering.

---

