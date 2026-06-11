# 🎬 Movie Explorer Website

A modern React-based Movie Explorer application built using **React.js**, **Material UI (MUI)**, **TMDB API**, **React Router**, **useReducer**, and **Local Storage**.

The application allows users to browse movies from multiple TMDB categories, view detailed movie information, discover similar movies, and maintain a personalized watchlist.

---

## 🚀 Features

### 🏠 Home Page

Displays movies in the following TMDB categories:

- 🎬 Now Playing
- 🌟 Popular
- 🏆 Top Rated
- ⏳ Upcoming

Each section displays:

- Movie Poster
- Movie Title
- Movie Rating

Movies are displayed in responsive card layouts with smooth navigation.

---

### 📄 Movie Details Page

When a user clicks a movie card, detailed information is displayed:

- Movie Poster
- Movie Title
- Rating
- Overview
- Cast Members
- Director Information

Additional Features:

- ➕ Add to My List
- ➖ Remove from My List
- 🎞 Similar Movies Section

---

### 📌 My List

Users can save movies to their personal watchlist.

Features:

- Persistent storage using Local Storage
- View saved movies anytime
- Remove movies from the list
- Displays:
  - Poster
  - Title
  - Rating

---

### 🔄 Similar Movies

Shows related movies using TMDB Similar Movies API.

Each movie card contains:

- Poster
- Title
- Rating

---

### 🛡 Error Handling

The application includes robust error handling.

If TMDB API requests fail:

- Fallback JSON data is loaded automatically.
- Application continues functioning without crashing.

---

### 💾 Local Storage

Watchlist data is stored in browser Local Storage.

Benefits:

- Data persists after page refresh.
- No backend required.

---

## 🛠 Tech Stack

### Frontend

- React.js
- React Router DOM
- Material UI (MUI)

### State Management

- useReducer
- Context API

### API

- TMDB (The Movie Database)

### Storage

- Browser Local Storage

### Build Tool

- Vite

---

## 📂 Project Structure

```text
src/
│
├── components/
│   ├── Sidebar.jsx
│   ├── MovieCard.jsx
│   ├── MovieSection.jsx
│   └── Header.jsx
│
├── pages/
│   ├── Home.jsx
│   ├── MyList.jsx
│   └── MovieDetails.jsx
│
├── context/
│   └── MovieListContext.jsx
│
├── api/
│   └── tmdb.js
│
├── App.jsx
├── main.jsx
└── index.css
