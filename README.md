## 📌 Project Overview:
F&Q Generator is an intelligent, high-retention learning tool that transforms raw lecture notes, text summaries, and PDF documents into interactive 3D flashcards and practice quizzes in seconds. Built with a responsive, modern "Afterparty" brutalist aesthetic, it leverages Google's Gemma 4 model to synthesize complex academic materials into bite-sized, active-recall study packs.

## The Problem:
*Passive Reading Fallacy: Students waste hours highlighting text and re-reading notes—methods proven to have low retention rates.
*High Setup Barrier: Manual flashcard creation in tools like Anki or Quizlet is tedious and consumes valuable study time.
*Complex UI Bloat: Existing flashcard apps are often cluttered, paywalled, or require heavy server installations.

## The Solution:
Instant Synthesis: Automatically parses raw text and multi-page PDFs locally in the browser.
Active Recall & Spaced Review: Formats content into high-impact question/answer pairs and multiple-choice quizzes with detailed explanations.
Zero-Backend Portability: Single-page application (SPA) architecture running directly in the browser—fast, private, and lightweight.
Seamless Interoperability: Allows instant export to Anki (CSV) for spaced repetition or structured JSON for custom workflows.

## Key Features:
In-Browser PDF & Text Parsing: Built-in client-side text extraction using pdf.js with drag-and-drop support.
AI Synthesis via Gemma 4: Powered by Google's gemma-4-26b-a4b-it model to generate contextual questions, distractors, and explanations.
Self-Paced Card Mastery: Track known vs. review-needed cards with visual progress indicators and status bars.
Interactive Practice Quiz Mode: Multiple-choice quiz interface featuring instant option validation, rationale explanations, and live score tracking.
Local Study Pack History: Automatically saves generated decks to local storage (up to 20 packs) for quick review.
Anki & JSON Export: Export study packs directly into Anki-ready CSV format or clean JSON schemas.

## Tech Stack: 
* Frontend Core:** HTML5, JavaScript (ES6+)
* Styling & Design:** Tailwind CSS (CDN Edition), Custom CSS 3D Transforms
* Typography & Icons:** FontAwesome 6, Google Fonts (*Plus Jakarta Sans*, *JetBrains Mono*)
* Document Processing:** PDF.js v3.11 (`pdf.worker.min.js`)
* AI Model & Inference:** Google Gemini API / Gemma 4 (`gemma-4-26b-a4b-it`)
* Storage & Exports:** Browser LocalStorage, Blob CSV/JSON Downloaders

## Setup & Installation:
 I) Prerequisites
 *Any modern Web Browser (Chrome, Firefox, Edge, Safari).
 *A Google Gemini API Key (with access to gemma-4-26b-a4b-it or Gemini models).
 II) Installation Steps
  1)Clone the Repository:
  git clone https://github.com/your-username/FlashCard_Hactober2026.git
  cd FlashCard_Hactober2026
  
  2)Configure API Key:
  Create a config.js file in the root directory:
  const CONFIG = {
    GEMINI_API_KEY: "YOUR_ACTUAL_GEMINI_API_KEY"
  };
  
  3)Run the Project:
  Simply open index.html in your favorite web browser, or launch it using a local development server (e.g., VS Code Live Server):
  Using Python simple HTTP server (optional)
  python -m http.server 8000

  ## Some Keyboard shortcuts that are useful:
  Space : Flip Flashcard

  →: Next Flashcard
  
  ←: Previous Flashcard

  Esc:Close open modal (About / Export / Packs)
## LICENSE 📄:

This project is licensed under the [MIT License](LICENSE) — created for Hacktoberfest 2026.

