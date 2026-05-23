  # Module 1 — What is HTML?

## Learning Objectives

By the end of this module, students will be able to:

1. Explain in plain English what HTML is and what it does
2. Describe the three layers of a webpage (HTML, CSS, JavaScript)
3. Write a valid HTML5 boilerplate from memory without referencing notes
4. Explain the purpose of every line in the boilerplate
5. Create a basic webpage with a heading and two paragraphs
6. Open a webpage in Chrome and view its source code
7. Identify the difference between tags, elements, and attributes

---

## Prerequisite Knowledge

None. This is the first module. Students do not need any prior coding experience.

---

## Concept Map

```
What is a webpage?
    ↓
Three layers: HTML + CSS + JavaScript
    ↓
What is HTML? (HyperText Markup Language)
    ↓
Tags → Elements → Attributes
    ↓
The HTML boilerplate (required structure)
    ↓
Head section vs Body section
    ↓
Your first working webpage
```

---

## Lesson Notes

### Concept 1 — What is a Webpage Made Of?

When you open any website in your browser, you're looking at three layers working together:

| Layer | Technology | Analogy |
|---|---|---|
| Structure | HTML | The walls, floors, and rooms of a house |
| Appearance | CSS | The paint, furniture, and decoration |
| Behaviour | JavaScript | The light switches, doors, and appliances |

We start with HTML because you cannot decorate a house that hasn't been built yet.

---

### Concept 2 — What is HTML?

HTML stands for **HyperText Markup Language**.

- **HyperText** = text that can link to other text (hyperlinks!)
- **Markup** = adding labels to content to describe what it IS
- **Language** = a set of rules the browser understands

Think of HTML tags like labels on folders in a filing cabinet.
You write `<p>` to tell the browser: "this content is a paragraph."
The browser reads that label and knows how to display it.

HTML does NOT control how things look — that is CSS's job.
HTML only controls what things ARE and where they are in the document.

---

### Concept 3 — Tags, Elements, and Attributes

**A tag** is the label itself:
```
<p>       ← opening tag
</p>      ← closing tag
```

**An element** is the opening tag + content + closing tag:
```
<p>This is a paragraph.</p>
```

**An attribute** gives extra information to an element:
```
<a href="/about">About us</a>
     ↑
     attribute: href="value"
```

Some elements are self-closing (they have no content):
```html
<img src="photo.jpg" alt="Description">
<input type="text">
<br>
<hr>
```

---

### Concept 4 — The HTML Boilerplate

Every HTML file must start with the same structure.
This is called the "boilerplate" — the required foundation every page is built on.

```html
<!DOCTYPE html>
<html lang="en">
  <head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <title>My First Page</title>
    <link rel="stylesheet" href="style.css">
  </head>
  <body>

    <h1>Hello, World!</h1>
    <p>This is my first webpage.</p>

  </body>
</html>
```

**Line-by-line breakdown:**

| Line | What it does | What happens if you leave it out |
|---|---|---|
| `<!DOCTYPE html>` | Tells browser this is HTML5 | Browser enters "quirks mode" — weird rendering |
| `<html lang="en">` | Root container for the whole page | Page may not be identified as English |
| `<meta charset="UTF-8">` | Enables all characters and emoji | Special characters show as ??? |
| `<meta name="viewport" ...>` | Fixes mobile display | Page appears zoomed out on phones |
| `<title>` | Browser tab text + search engine title | Tab shows the URL instead |
| `<link rel="stylesheet">` | Connects your CSS file | No styles apply |
| `<body>` | Container for all visible content | Nothing shows in the browser |

---

### Concept 5 — Head vs Body

```
<head> = information ABOUT the page (not visible to users)
  - The page title (shown in tab)
  - Links to CSS files
  - Meta information for search engines and browsers

<body> = everything VISIBLE on the page
  - Headings, paragraphs, images, links
  - Navigation, sections, forms
  - Everything the user actually sees
```

---

## Exercises

### Exercise 1-A — The Boilerplate (Guided)

**Goal:** Create your first valid HTML file from scratch.

**Instructions:**
1. Open VS Code
2. Create a new file called `index.html` inside your `student-projects/your-name/` folder
3. Type (do NOT copy-paste) the boilerplate exactly as shown above
4. Change the `<title>` to: `[Your Name] — My First Page`
5. Change the `<h1>` to: `Hello, I'm [Your Name]`
6. Add a `<p>` tag with one sentence about where you're from
7. Add another `<p>` with one sentence about why you want to learn web development
8. Save the file (Ctrl+S)
9. Right-click the file in VS Code → "Open with Live Server"
10. Take a screenshot of your browser showing the page

**Expected result:** A white page with your heading and two paragraphs.

---

### Exercise 1-B — View Source (Guided)

**Goal:** See the HTML behind a real website.

**Instructions:**
1. Open Google.com in Chrome
2. Press `Ctrl+U` (Windows) or `Cmd+Option+U` (Mac)
3. A new tab opens showing the page's HTML source code
4. Find the `<title>` tag — what does it say?
5. Find the `<body>` tag
6. Close the source tab
7. Right-click on the Google logo → "Inspect"
8. The DevTools panel opens — hover over different elements
9. Notice how each element highlights in the browser

**Discussion question:** What HTML elements can you recognize?

---

### Exercise 1-C — Tags and Elements (Semi-Guided)

**Goal:** Practice identifying HTML components.

Given this HTML, answer the questions:

```html
<a href="https://github.com" target="_blank">Visit GitHub</a>
```

Questions:
1. What is the opening tag?
2. What is the closing tag?
3. What is the element name?
4. What are the two attributes?
5. What is the content of this element?
6. What does `target="_blank"` probably do? (Guess before looking it up)

---

### Exercise 1-D — Milestone Practice

**Goal:** Type the boilerplate from memory.

Close all notes and tabs showing the boilerplate.
Type it from memory in a new blank file.
Then compare with the original — how accurate were you?

Repeat until you can write it without looking.
This is your Module 1 milestone requirement.

---

## Common Mistakes

| Mistake | How to Spot It | How to Fix It |
|---|---|---|
| Missing DOCTYPE | Page renders oddly in some browsers | Add `<!DOCTYPE html>` as the very first line |
| No closing tag | Content "bleeds" into the next element | Every `<opening>` needs a `</closing>` |
| Tags not lowercase | `<P>`, `<H1>` | HTML is lowercase: `<p>`, `<h1>` |
| Missing quotes on attributes | `href=about` | Always: `href="about"` |
| Content outside `<body>` | Unpredictable rendering | Everything visible goes inside `<body>` |

---

## Milestone Assessment

**Requirement to advance to Module 2:**

In front of the instructor (or recorded video), demonstrate:
1. Open a blank file in VS Code
2. Type the complete HTML boilerplate from memory (no notes, no autocomplete)
3. Explain out loud what each line does as you type it
4. Add a heading, two paragraphs, and a link to the file
5. Open it in Chrome and confirm it displays correctly

The boilerplate must be 100% correct. The explanation must cover all 7 required elements.
