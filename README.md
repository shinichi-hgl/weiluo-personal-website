# Wei Luo's Academic Personal Website

This repository hosts the personal academic portfolio website of Dr. Wei Luo, Assistant Professor at the School of Government, Peking University. 

*   **Live Website URL:** [https://wei-luo.com/](https://wei-luo.com/)
*   **Hosting Platform:** GitHub Pages (automatic deployment on every push to the `main` branch).

---

## 📂 Project Structure

This project uses a clean, zero-dependency **HTML5 / Vanilla CSS / Vanilla JS** architecture. It has no build steps or compile processes, making it highly portable, fast, and easy for AI tools to modify.

*   `index.html` — The main landing page (About, Research overview, timeline, contact form).
*   `styles.css` — Central stylesheet defining layout, light/dark themes, and responsive views.
*   `script.js` — Interactive actions (theme toggling, publication filtering, expanding abstracts).
*   `robots.txt` — Welcomes search engines and AI crawlers (like OpenAI's OAI-SearchBot and Perplexity).
*   `sitemap.xml` — Declares all public URLs to crawlers to ensure visibility.
*   `avatar.jpg` — Profile picture.
*   `publications/` — Directory containing dedicated, SEO-optimized pages for each research paper:
    *   `taming-violence.html`
    *   `relational-work.html`
    *   `glauthoritarian-urbanization.html`
    *   `ladies-vanish-wikipedia.html`

---

## 🤖 Guide: How to Edit This Website Using AI Tools

If you are using an AI coding assistant (like Gemini, ChatGPT, Claude, or cursor.sh), you can copy-paste the instructions below to tell the AI how to edit this codebase without breaking anything.

### Copy-Paste Prompt Templates for AI:

#### 1. To Add a New Publication:
> "I have a new academic publication. Please add it to my website.
> 1. Create a new file in `publications/your-paper-title.html` modeled on the existing publication pages.
> 2. Ensure you fill in the Google Scholar meta tags (`citation_title`, `citation_author`, etc.) in the `<head>`.
> 3. Add a structured JSON-LD `ScholarlyArticle` schema to the new page.
> 4. Write an AI-readable summary section (Research Question, Argument, Methods, Key Findings, Contribution).
> 5. Add the paper to the list in `index.html` under the appropriate categories.
> 6. Update `sitemap.xml` to include the new page URL.
> Here is the details of my paper: [Paste paper info here]"

#### 2. To Update Bio or Contact Info:
> "Please update my biography and office address on my website. Modify both the visual text in `index.html` and the JSON-LD structured data in the `<head>` of `index.html` to keep them synchronized. Here are the new details: [Paste details here]"

#### 3. To Change Website Themes or Colors:
> "I want to change the primary colors of my website. Open `styles.css` and modify the custom CSS properties inside `:root` (for the Light Theme) and `[data-theme="dark"]` (for the Dark Theme). Please use a harmonious academic color scheme. [Specify colors or style preferences here]"

---

## 🚀 How to Run and Deploy Changes

### 1. View the website locally
Since there are no build steps, you can double-click `index.html` to open it in your browser, or run a simple local server from the project directory:
```bash
python3 -m http.server 8080
```
Then visit `http://localhost:8080`.

### 2. Save and Publish Updates
Once you or your AI assistant makes changes to the files, run these commands in your terminal to deploy them live:

```bash
# 1. Stage all changes
git add .

# 2. Save the changes with a description
git commit -m "Update website content"

# 3. Publish it live to GitHub Pages
git push
```
*(Changes will go live automatically on GitHub Pages within 30–60 seconds).*
