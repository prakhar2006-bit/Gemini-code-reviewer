# Gemini Code Reviewer

An AI-powered code review application built with React and Google's Gemini 2.5 Flash model. Get instant, professional-level feedback on your code including bug detection, security vulnerabilities, performance suggestions, and best practices.

![Powered by Gemini](https://img.shields.io/badge/Powered%20by-Google%20Gemini-blue)
![React](https://img.shields.io/badge/React-19.1.0-61DAFB)
![TypeScript](https://img.shields.io/badge/TypeScript-5.7-3178C6)
![Vite](https://img.shields.io/badge/Vite-6.2-646CFF)

## ✨ Features

- **Multi-Language Support**: Review code in 15+ programming languages including:
  - JavaScript, TypeScript, Python, Java, C#, Go, Rust, Ruby, PHP, Kotlin, Swift, C++, HTML, CSS, SQL

- **Comprehensive Code Analysis**:
  - 🐛 **Bug Detection**: Identifies logical errors, off-by-one errors, null pointer exceptions, and runtime issues
  - 🔒 **Security Vulnerabilities**: Detects injection attacks, XSS, insecure data handling, and more
  - ⚡ **Performance Optimization**: Suggests ways to improve speed and memory efficiency
  - 📖 **Readability & Best Practices**: Reviews code style, naming conventions, and language-specific practices
  - 🔧 **Maintainability**: Assesses code structure and extensibility

- **Structured Feedback**: Organized review output with:
  - Overall summary of code quality
  - Issues categorized by severity (Critical, High, Medium, Low)
  - Suggestions categorized by type (Performance, Readability, Best Practice, Security)
  - Actionable code snippets for fixes

- **User-Friendly Interface**:
  - Clean, modern dark theme UI
  - Side-by-side code input and review output
  - Copy-to-clipboard functionality for suggestions
  - Responsive design for all screen sizes

## 🚀 Getting Started

### Prerequisites

- Node.js (v18 or higher recommended)
- A Google Gemini API key

### Installation

1. **Clone the repository**:
   ```bash
   git clone https://github.com/nitinog10/Gemini-code-reviewer.git
   cd Gemini-code-reviewer
   ```

2. **Install dependencies**:
   ```bash
   npm install
   ```

3. **Set up environment variable**:
   
   Create a `.env` file in the root directory and add your Gemini API key:
   ```env
   API_KEY=your_gemini_api_key_here
   ```
   
   > Get your API key from [Google AI Studio](https://aistudio.google.com/app/apikey)

4. **Start the development server**:
   ```bash
   npm run dev
   ```

5. **Open your browser** and navigate to the URL shown in the terminal (typically `http://localhost:5173`)

## 📦 Scripts

| Command | Description |
|---------|-------------|
| `npm run dev` | Start development server with hot reload |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build locally |

## 🏗️ Project Structure

```
Gemini-code-reviewer/
├── components/
│   ├── CodeInput.tsx        # Code input textarea component
│   ├── Header.tsx           # Application header with logo
│   ├── LanguageSelector.tsx # Programming language dropdown
│   ├── Loader.tsx           # Loading spinner component
│   ├── ReviewOutput.tsx     # Displays formatted review results
│   └── icons/               # SVG icon components
│       ├── CheckIcon.tsx
│       ├── ClipboardIcon.tsx
│       └── SparklesIcon.tsx
├── services/
│   └── geminiService.ts     # Gemini API integration
├── App.tsx                  # Main application component
├── constants.ts             # Language options configuration
├── types.ts                 # TypeScript type definitions
├── index.tsx                # Application entry point
├── index.html               # HTML template
├── vite.config.ts           # Vite configuration
├── tsconfig.json            # TypeScript configuration
└── package.json             # Project dependencies
```

## 🔧 Tech Stack

- **Frontend**: React 19.1 with TypeScript
- **Build Tool**: Vite 6.2
- **AI Model**: Google Gemini 2.5 Flash
- **Styling**: Tailwind CSS
- **API Client**: @google/genai

## 💡 How It Works

1. **Paste your code** in the left panel
2. **Select the programming language** from the dropdown
3. **Click "Review Code"** to submit for analysis
4. **Receive structured feedback** including:
   - A brief summary of code quality
   - List of issues with severity levels and fix suggestions
   - Improvement recommendations with code snippets

## 🤝 Contributing

Contributions are welcome! Feel free to:
- Report bugs
- Suggest new features
- Submit pull requests

## 📄 License

This project is open source and available under the [MIT License](LICENSE).

## 🙏 Acknowledgments

- Powered by [Google Gemini](https://deepmind.google/technologies/gemini/)
- Built with [React](https://react.dev/) and [Vite](https://vitejs.dev/)