# Polyglot Flashcards

A modern, single-page web application (SPA) designed for language learners to manage vocabulary lists efficiently. This project supports multiple languages, custom categorization, dark mode, and a robust JSON Export/Import system for data portability.

It runs entirely in the browser using LocalStorage, requiring no backend setup.

## Features

### Multi-Language Architecture
* **Independent Environments:** Create separate vocabulary lists for different languages (e.g., English, German, Spanish).
* **Context Switching:** Seamlessly switch between languages without reloading the page. Data and categories are isolated per language.

### Dynamic Theme System
* **Dark & Light Mode:** Built-in theme switcher utilizing Bootstrap 5's color modes.
* **Adaptive UI:** Card borders and backgrounds adjust dynamically (Dark Grey borders for Light Mode, White borders for Dark Mode) to ensure optimal readability.

### Data Management & Portability
* **JSON Export:** Download vocabulary lists and category structures for the current language as a .json file.
* **JSON Import:** Restore backups or merge external datasets into the existing application state.
* **LocalStorage Persistence:** All data is saved automatically to the browser, ensuring data remains available across sessions.

### Content Organization
* **CRUD Operations:** Create, Read, Update, and Delete flashcards instantly.
* **Category Manager:** Add, edit, or remove custom tags (e.g., "Grammar", "Phrasal Verbs") via a dedicated modal interface.
* **Advanced Filtering:** Filter visible cards based on creation time (Today, This Week, All Time) or specific categories.

## Technologies Used

* **HTML5:** Semantic structure.
* **CSS3:** Custom animations (3D Flip effects) and responsive layout.
* **Bootstrap 5:** UI components, grid system, and theme management.
* **jQuery:** DOM manipulation, event handling, and application logic.
* **Bootstrap Icons:** Iconography.


## Data Structure Specification

The application exports data in a specific JSON structure. This format can be used to generate flashcard sets programmatically.

```json
{
  "language": "English",
  "date": "2026-01-09T18:00:00.000Z",
  "categories": [
    "General",
    "Verbs",
    "Idioms"
  ],
  "cards": [
    {
      "id": 1704829200000,
      "front": "Ephemeral",
      "back": "Lasting for a very short time.",
      "category": "General",
      "createdAt": "2026-01-09T10:00:00.000Z"
    }
  ]
}
