REACT CHATBOT2.0

This is a simple, interactive chatbot application built with React, leveraging the Google Gemini API for conversational AI. The project provides a clean user interface where users can ask questions and receive responses from a powerful language model.

✨ Features
Real-time Chat: Send messages and receive instant responses from the Gemini AI.

New Chat: Start a fresh conversation by clearing the current chat history.

Copy Chat: Easily copy the entire conversation log to your clipboard.

Responsive Design: A basic layout designed for a modern web experience.

🚀 Technologies Used

React: A JavaScript library for building user interfaces.

Vite: A fast build tool that provides a rapid development experience.

Google Gemini API (via @google/generative-ai): Powers the conversational AI capabilities.

CSS: For styling and layout.

⚙️ Setup and Installation

Follow these steps to get the project up and running on your local machine.

1. Clone the Repository (or initialize if starting from scratch)
If you're starting from scratch as per the previous steps, you've already created the project. If you were cloning an existing one, you'd do:

git clone https://github.com/your-username/chatbot-react.git # Replace with your repo URL
cd chatbot-react

2. Install Dependencies
Navigate into the project directory and install the necessary Node.js packages:

npm install

This will install react, react-dom, @google/generative-ai, and other development dependencies.

3. Obtain Your Google Gemini API Key
To use the chatbot, you need an API key for the Google Gemini API:

Go to Google AI Studio or the Google Cloud Console.

Follow the instructions to create a new API key for the Gemini API.

4. Configure Environment Variables
Create a new file named .env in the root directory of your project (same level as package.json):

VITE_GEMINI_API_KEY=YOUR_API_KEY_HERE

Replace YOUR_API_KEY_HERE with the actual API key you obtained in the previous step.

Important: The .env file should not be committed to version control. It's already included in .gitignore by default in Vite projects.

5. Run the Development Server
Once the dependencies are installed and your API key is configured, you can start the development server:

npm run dev

This command will typically open your browser to http://localhost:5173/ (or another available port) where you can interact with the chatbot.

💡 Usage

Type a message: Enter your question or prompt into the input field at the bottom of the chat window.

Send message: Press Enter or click the "Send" (arrow) button to send your message.

New Chat: Click "New Chat" in the left sidebar to clear the conversation and start over.

Copy Chat: Click "Copy" in the top right of the chat window to copy the entire chat history to your clipboard.

👨‍💻 Project Structure
chatbot-react/
├── public/                     # Public assets (e.g., favicon)
├── src/
│   ├── components/
│   │   ├── ChatApp.jsx         # Main layout component
│   │   ├── ChatWindow.jsx      # Chat messages display and input logic
│   │   └── Sidebar.jsx         # Left-hand navigation sidebar
│   ├── App.jsx                 # Root React component
│   ├── main.jsx                # Entry point for React application
│   └── styles.css              # Global CSS styles
├── .env                        # Environment variables (for API key)
├── .gitignore                  # Git ignore rules
├── index.html                  # Main HTML file
├── package.json                # Project dependencies and scripts
└── README.md                   # This file

🔮 Future Enhancements

User Authentication: Implement user login to save chat history.

Theming Options: Allow users to switch between light/dark modes or other themes.

Message Formatting: Support Markdown rendering for bot responses.

Error Boundaries: More robust error handling for API failures.

Load Previous Chats: Store and retrieve past conversations.

Typing Indicator: A more dynamic typing indicator for the bot.

📄 License

This project is open-source and available under the MIT License.
