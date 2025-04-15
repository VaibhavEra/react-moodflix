# Moodflix

Moodflix is a React-based website project designed to help beginners get started with learning React.js. The platform offers a sleek and modern experience for browsing and discovering movies.

## 🔋 Features

- 👉 **Browse All Movies**: Explore a wide range of movies available on the platform.
- 👉 **Search Movies**: Easily search for specific movies using a search function with debounced input.
- 👉 **Trending Movies Algorithm**: Displays trending movies based on search popularity.
- 👉 **Modern UI/UX**: A sleek and user-friendly interface designed for a great experience.
- 👉 **Responsiveness**: Fully responsive design that works seamlessly across devices.

## 🛠️ Tech Stack

- **React.js**: Frontend library for building the user interface
- **Appwrite**: Backend service for the Trending Movies Algorithm and data storage
- **Tailwind CSS**: Utility-first CSS framework for styling
- **TMDB API**: Movie database API for fetching movie information
- **react-use**: For utility hooks like useDebounce

## 📦 Project Structure

The project includes several key components:

- **App Component**: Core application with TMDB API integration and movie discovery functionality
- **Search Component**: User interface for searching movies with debounced input
- **MovieCard Component**: Display card for individual movies with details like rating, language, and release year
- **Spinner Component**: Loading indicator for asynchronous operations
- **Appwrite Integration**: Backend service for tracking search terms and generating trending movies

## 🚀 Getting Started

### Prerequisites

- Node.js (v14 or higher)
- npm or yarn
- Appwrite account

### Installation

1. Clone the repository:

   ```bash
   git clone git@github.com:VaibhavEra/react-moodflix.git
   cd react-moodflix
   ```

2. Install dependencies:

   ```bash
   npm install
   # or
   yarn install
   ```

3. Create a `.env` file in the root directory and add your API keys:

   ```
   VITE_TMDB_API_KEY=your_tmdb_api_key
   VITE_APPWRITE_PROJECT_ID=your_appwrite_project_id
   VITE_APPWRITE_DATABASE_ID=your_appwrite_database_id
   VITE_APPWRITE_COLLECTION_ID=your_appwrite_collection_id
   ```

4. Start the development server:

   ```bash
   npm run dev
   # or
   yarn dev
   ```

5. Open [http://localhost:5173](http://localhost:5173) to view the app in your browser.

## 🧩 Key Components

### App Component

The main component that orchestrates the application:

- Manages state for movies, search terms, loading states
- Implements debounced search for better performance
- Fetches movies from TMDB API
- Displays trending movies from Appwrite

### MovieCard

Displays individual movie information including:

- Movie poster (with fallback image)
- Title
- Rating (with star icon)
- Original language
- Release year

### Appwrite Integration

Provides backend functionality:

- `updateSearchCount`: Tracks search terms and their frequency
- `getTrendingMovies`: Retrieves most popular searches for trending section
- Stores movie metadata for display purposes

## 🙏 Acknowledgements

- [TMDB API](https://www.themoviedb.org/documentation/api) for providing movie data
- [Vite](https://vitejs.dev/) for the blazing fast development experience
- [Tailwind CSS](https://tailwindcss.com/) for the utility-first CSS framework
- [Appwrite](https://appwrite.io/) for backend services
