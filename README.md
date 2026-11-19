# Blog Site

A blog application built using React, React Router, Axios, and Tailwind CSS, with a REST API for managing blog posts.

## Features

- **Post Feed:** Browse blog posts with titles, dates, and descriptions.
- **Article View:** Read individual blog posts.
- **Create Posts:** Add new blog posts through a form.
- **Edit Posts:** Update existing blog post content.
- **Delete Posts:** Remove blog posts.
- **Client-Side Routing:** Navigate between pages using React Router.
- **About Page:** A separate page with information about the application.
- **404 Page:** Handles unknown routes.

## Technologies Used

- React
- JavaScript
- React Router
- Axios
- Tailwind CSS
- JSON Server

## Getting Started

### Prerequisites

- Node.js
- npm

### Installation

1. Clone the repository:

   ```bash
   git clone https://github.com/charankumaregd/blog-site.git
   cd blog-site
   ```

2. Install dependencies:

   ```bash
   npm install
   ```

### Running the Application

The application uses a local REST API powered by JSON Server.

1. Start the mock API server in a terminal:

   ```bash
   npx json-server --watch src/db/posts.json --port 3500
   ```

2. Open another terminal and start the React application:

   ```bash
   npm start
   ```

3. Open `http://localhost:3000` in your browser.

## Project Structure

```text
blog-site/
├── public/
├── src/
│   ├── api/
│   │   ├── Axios.js
│   │   └── crud.js
│   ├── components/
│   │   ├── Footer.jsx
│   │   ├── Header.jsx
│   │   ├── Navbar.jsx
│   │   └── Post.jsx
│   ├── db/
│   │   └── posts.json
│   ├── pages/
│   │   ├── About.js
│   │   ├── EditPost.js
│   │   ├── Home.js
│   │   ├── NewPost.js
│   │   ├── NotFound.js
│   │   └── Post.js
│   ├── App.js
│   ├── Layout.js
│   ├── index.css
│   └── index.js
├── package.json
├── package-lock.json
├── tailwind.config.js
└── README.md
```

## Implementation Notes

- React Router handles client-side navigation and nested routes.
- Axios is used to communicate with the REST API.
- JSON Server provides a local mock backend for storing blog posts.
- Blog post data is maintained in `src/db/posts.json`.