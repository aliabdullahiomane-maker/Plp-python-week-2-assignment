# Personal Budget & Expense Tracker (Week 2)

A simple static Personal Budget & Expense Tracker built with HTML and CSS. This project extends the Week 1 skeleton by adding an expense table, an improved form, multimedia content, and interactive elements.

## What I built

- A main page with:
  - A header with a money icon and title
  - A budget summary section (Total Income, Total Expenses, Balance)
  - A Budgeting Tips section with an embedded YouTube video
  - A collapsible “How to use this tracker” instructions section
  - An “Add Expense” form with:
    - Expense name
    - Amount
    - Category dropdown (Food, Transport, Rent, Entertainment, Other)
  - A “Your Expenses” table with 5 sample expenses (Name, Amount, Category, Date)

## Files in this repository

- `index.html`  
  Contains the HTML structure:
  - Header with logo (`<img>`)
  - Summary cards
  - Video section (`<iframe>`)
  - Instructions using `<details>` and `<summary>`
  - Add Expense form inside `<section id="add-expense">`
  - Your Expenses table inside `<section id="your-expenses">`

- `style.css`  
  Contains all visual styling:
  - Global reset and base styles
  - Styling for cards, forms, tables, header, footer
  - Table styles:
    - `border-collapse: collapse`
    - Cell padding and borders
    - Colored header row
    - Alternating row colours with `tr:nth-child(even)`
    - Hover effect on table rows
  - Advanced CSS selectors:
    - Descendant selector: `#your-expenses td`
    - Direct child selector: `.expense-form > input`
    - Position pseudo-class: `tr:nth-child(even)`, `tr:first-child`
    - Negation pseudo-class: `input:not([type="submit"])`
    - Focus state: `input:focus`, `select:focus`

- `money.png`  
  Small money icon displayed next to the main heading in the header.

- `README.md`  
  This file – explains what the project is and what each part does.

## How to run the project

1. Clone or download this repository to your computer.
2. Open the project folder in VS Code (or any code editor).
3. Open `index.html` in your browser:
   - Double‑click the file, or
   - Use “Open with Live Server” in VS Code if you have that extension.

You should see the budget tracker with styled sections, a table of sample expenses, an embedded video, and collapsible instructions.

## Notes

- The “Add Expense” button does not save or add new rows yet. It is prepared with proper IDs and structure for JavaScript in later weeks.
- This project demonstrates:
  - Semantic HTML (headings, sections, forms, tables, details/summary)
  - CSS selectors (element, class, ID, and advanced selectors)
  - Multimedia embedding (`<img>`, `<iframe>`)
  - Basic interactive content (`<details>` and `<summary>`)
