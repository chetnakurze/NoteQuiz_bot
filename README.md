# NoteQuiz Bot ✦

An intelligent, browser-based study assistant and active recall quiz generator. **NoteQuiz** turns lecture notes, study guides, and presentation documents into focused quizzes with customizable question types, difficulty levels, and instant answer keys.

---

## ✨ Features

- **Document Ingestion (In-Browser & Private)**:
  - Supports **PDF**, **DOCX** (via Mammoth.js), **PPTX** (via JSZip), **TXT**, and **Markdown** files.
  - Drag-and-drop file upload with zero server uploads—all parsing runs directly inside your browser.
  - Direct paste option for quick lecture snippets or summaries.
- **Customizable Quizzes**:
  - **Question Types**: Mixed, Multiple Choice, Short Answer, Long Answer, True / False, and Fill in the Blank.
  - **Difficulty Levels**: Easy, Medium, and Hard.
  - **Question Count**: Select 3, 5, or 8 questions per quiz.
- **Interactive Study Interface**:
  - Full answer key toggle (show/hide answers).
  - One-click quiz regeneration on the same material.
  - Contextual Q&A: Ask questions directly about your uploaded material (e.g. *"Explain semantic segmentation"*).
- **Study Chat History**:
  - Save and organize study sessions across different lectures or topics.
  - Search your study chat history easily.
  - Persistent storage using browser `localStorage`.

---

## 🚀 Getting Started

No build step or external dependencies required! You can run NoteQuiz directly in any modern web browser.

### Option 1: Open Directly
Simply double-click `index.html` or open it in your browser.

### Option 2: Run with a Local Static Server
You can also serve the files using any simple HTTP server:

Using Python:
```bash
python -m http.server 8000
```
Then open [http://localhost:8000](http://localhost:8000) in your browser.

Or using Node.js / `npx`:
```bash
npx serve .
```

---

## 📂 Project Structure

```text
├── index.html       # Main application layout and semantic markup
├── styles.css       # Core typography, color system, and layout styles
├── upload.css       # Drag-and-drop upload zone styling & transitions
├── app.js           # Client-side logic: file parsing, question generation, Q&A, and history
├── .gitignore       # Git ignore rules for temporary and checkpoint files
└── README.md        # Project documentation
```

---

## 🛠️ Built With

- **HTML5 & CSS3** (Custom design system with DM Sans & Fraunces fonts)
- **Vanilla JavaScript** (Modern ES6+)
- [PDF.js](https://mozilla.github.io/pdf.js/) for in-browser PDF parsing
- [Mammoth.js](https://github.com/mwilliamson/mammoth.js) for DOCX extraction
- [JSZip](https://stuk.github.io/jszip/) for PPTX slide parsing

---

## 📄 License

Open-source under the [MIT License](LICENSE).
