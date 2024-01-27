## Introduction

This is a simple React-based movie application that allows users to explore popular, top-rated, and upcoming movies. It utilizes The Movie Database (TMDb) API to fetch movie data and display it in various views.

## Project Structure

The project is organized into several folders:

### `Public` Folder

The `public` folder contains static assets and the main HTML file:

- **index.html**: The main HTML file that serves as the entry point for the React application. It includes metadata, links to stylesheets, and the root `<div>` where the React app is mounted.

### `SRC` Folder

The `src` folder contains the source code of the React application, organized into subfolders:

#### `Components` Folder

1. **Card.js**: A React component (`Cards`) responsible for rendering individual movie cards. It uses the `react-loading-skeleton` library to display loading skeletons while fetching movie data.

2. **Header.js**: A React component (`Header`) representing the application header, including navigation links.

3. **MovieList.js**: A React component (`MovieList`) displaying a list of movies based on the selected category (popular, top-rated, upcoming).

#### `Pages` Folder

1. **Movie.js**: A React component (`Movie`) displaying detailed information about a specific movie. It fetches data from TMDb API based on the movie ID.

2. **Home.js**: A React component (`Home`) displaying a carousel of popular movies. It fetches data from the TMDb API for popular movies.

#### `App.js`

The main React component (`App`) responsible for setting up routes using React Router. It includes the application header and defines routes for the home page, movie details page, movie list page, and an error page.

#### `index.js`

The entry point of the React application, rendering the `App` component into the root `<div>` specified in the `index.html` file.

## Running the Application

To run the application locally:

1. Ensure you have Node.js and npm installed on your machine.
2. Clone the repository.
3. Navigate to the project directory in the terminal.
4. Run `npm install` to install dependencies.
5. Run `npm start` to start the development server.
6. Open your browser and go to [http://localhost:3000](http://localhost:3000) to view the application.

## Dependencies

- **React**: JavaScript library for building user interfaces.
- **React Router**: Declarative routing for React applications.
- **react-loading-skeleton**: A library for creating loading skeletons in React components.
- **react-responsive-carousel**: A responsive carousel component for React.
- **FontAwesome**: For including font icons in the application.

## API Integration

The application uses the TMDb API to fetch movie data. API key authentication is required, and it is currently included in the code. Note that API keys should be kept secure and not exposed in client-side code in a production environment.
