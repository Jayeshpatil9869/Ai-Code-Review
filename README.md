# AI Code Review Application

This project is a full-stack application that allows users to input code and receive AI-generated reviews. It consists of a **Frontend** built with React and Vite, and a **Backend** powered by Node.js and Express. The backend integrates with Google's Generative AI to provide detailed code reviews.

## Features

- **Code Editor**: A simple code editor with syntax highlighting.
- **AI Code Review**: Sends the code to the backend and receives AI-generated feedback.
- **Real-Time Rendering**: Displays the AI review in a markdown-styled output.

---

## Project Structure

### Frontend

- **Framework**: React
- **Build Tool**: Vite
- **Key Libraries**:
  - `react-simple-code-editor`: For the code editor.
  - `prismjs`: For syntax highlighting.
  - `react-markdown` & `rehype-highlight`: For rendering markdown with syntax highlighting.
  - `axios`: For making API requests.

**Directory Structure**:

```
Frontend/
├── public/               # Static assets
├── src/                  # Source code
│   ├── App.jsx           # Main application component
│   ├── App.css           # Styles for the app
│   ├── main.jsx          # Entry point
│   ├── index.css         # Global styles
│   └── assets/           # Additional assets
├── package.json          # Project dependencies and scripts
├── vite.config.js        # Vite configuration
└── index.html            # HTML template
```

### Backend

- **Framework**: Express
- **Key Libraries**:
  - `@google/generative-ai`: For integrating with Google's Generative AI.
  - `dotenv`: For environment variable management.
  - `cors`: For handling cross-origin requests.

**Directory Structure**:

```
BackEnd/
├── src/
│   ├── app.js            # Express app setup
│   ├── controllers/      # Route controllers
│   │   └── ai.controller.js
│   ├── routes/           # API routes
│   │   └── ai.routes.js
│   └── services/         # Business logic
│       └── ai.service.js
├── server.js             # Server entry point
├── .env                  # Environment variables
├── package.json          # Project dependencies and scripts
└── package-lock.json     # Dependency lock file
```

---

## Installation

### Prerequisites

- Node.js (v20 or higher)
- npm or yarn

### Backend Setup

1. Navigate to the `BackEnd` directory:
   ```bash
   cd BackEnd
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Create a `.env` file and add your Google Gemini API key:
   ```properties
   GOOGLE_GEMINI_KEY=your_api_key_here
   ```
4. Start the server:
   ```bash
   npm start
   ```
   The server will run on `http://localhost:3000`.

### Frontend Setup

1. Navigate to the `Frontend` directory:
   ```bash
   cd Frontend
   ```
2. Install dependencies:
   ```bash
   npm install
   ```
3. Start the development server:
   ```bash
   npm run dev
   ```
   The app will run on `http://localhost:5173`.

---

## Usage

1. Open the frontend in your browser.
2. Write or paste your code into the editor.
3. Click the **Review** button to send the code to the backend.
4. View the AI-generated review in the output panel.

---

## Environment Variables

The backend requires the following environment variable:

- `GOOGLE_GEMINI_KEY`: Your Google Generative AI API key.

---

## Scripts

### Backend

- `npm start`: Starts the backend server.

### Frontend

- `npm run dev`: Starts the development server.
- `npm run build`: Builds the production-ready app.
- `npm run preview`: Previews the production build.
- `npm run lint`: Runs ESLint to check for code issues.

---

## Dependencies

### Frontend

- `react`, `react-dom`: React library.
- `axios`: For API requests.
- `prismjs`: Syntax highlighting.
- `react-simple-code-editor`: Code editor component.
- `react-markdown`, `rehype-highlight`: Markdown rendering.

### Backend

- `express`: Web framework.
- `dotenv`: Environment variable management.
- `cors`: Cross-origin resource sharing.
- `@google/generative-ai`: Google Generative AI integration.

---
## 📽️ Demo

Watch the full demo of the AI Code Review Application:  
[![Watch Video](https://github.com/user-attachments/assets/63916764-cabc-440a-862d-2a5ddebe9109)



## License

This project is licensed under the ISC License.

---

## Acknowledgments

- [Google Generative AI](https://developers.google.com/ai)
- [React](https://reactjs.org/)
- [Vite](https://vitejs.dev/)
