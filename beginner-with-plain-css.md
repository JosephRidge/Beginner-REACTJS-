# Beginner Web Development with React: Plain CSS Track (8 Weeks)

This 8-week beginner course takes learners from HTML to a published React app, and every page and component is styled with ordinary CSS files, with no UI library.

**Other tracks:** [Tailwind track](../tailwind-track/README.md) · [Mid-level track](../mid-level-track/README.md) · [All tracks](../README.md)

## Contents

- [Course at a glance and strands](#course-at-a-glance-and-strands)
- [Week-by-week plan](#week-by-week-plan)
- [Styling in React with plain CSS](#styling-in-react-with-plain-css-week-6-session-3)
- [Build the feature, then improve the UI with AI](#session-build-the-feature-then-improve-the-ui-with-ai-week-7-session-4)
- [Assessment and resources](#assessment-and-resources)

## Course at a glance and strands

Learners spend four weeks on web basics, three on React, and one on a showcase project. In this track, CSS gets the most time in Week 2 and stays the only styling tool all the way to the capstone.

| Item | Detail |
| --- | --- |
| Duration | 8 weeks (assumed: 4 sessions a week, 3 hours each, about 96 hours) |
| Level | Absolute beginner; basic computer literacy and a laptop |
| Approach | Competency-based and project-based; about 30% short talks, 70% hands-on |
| Tools | VS Code, Chrome, Git and GitHub, Node.js with Vite, Netlify or GitHub Pages |
| Styling | Plain CSS files, CSS variables, Flexbox, Grid, and media queries |
| Exit outcome | Learner builds, styles, and publishes a small React app and explains how it works |

| Strand | Week | Sub-strand | Specific learning outcomes (by the end of the week the learner can…) |
| --- | --- | --- | --- |
| 1. Web foundations | 1 | How the web works; HTML | Explain browser, server, and URL; build a page with headings, images, links, lists, and a form |
| 2. Styling and layout | 2 | CSS, Flexbox, Grid, responsive design | Style text, colour, and spacing; lay out content with Flexbox and Grid; use CSS variables; make a page work on phone and laptop |
| 3. JavaScript | 3 | Core JavaScript; the DOM | Use variables, conditions, loops, and functions; react to clicks and change the page |
| 3. JavaScript | 4 | Modern JavaScript; Git; tools | Use arrays, map, filter, objects, arrow functions, and destructuring; commit, branch, and push with Git; start a Vite project |
| 4. Building with React | 5 | Components, JSX, props, className | Build reusable components; pass props; style with className and a CSS file; show content conditionally |
| 4. Building with React | 6 | State, events, lists, forms | Use useState; show lists with keys; build a controlled form; lift state up to share it |
| 4. Building with React | 7 | Effects and API data | Load data with useEffect and fetch; show loading and error messages; refine the UI with AI safely |
| 5. Project and practice | 8 | Capstone and deployment | Plan, build, publish, and present a React app with a README and a portfolio page |

## Week-by-week plan

Each week has a key inquiry question (KIQ), hands-on experiences, and a mini-project pushed to GitHub. Session 1 is a demo, Sessions 2 and 3 are guided pair practice, and Session 4 is the mini-project and peer review.

### Week 1: How the web works and HTML

- **KIQ:** What happens when I type a web address and press Enter?
- Role-play browser, server, and request; use "View Source" on a school or news site
- Build a profile page with headings, a photo with alt text, a list, links, and a contact form
- **Mini-project:** A one-page profile for the learner or a local group

### Week 2: CSS, layout and responsive design

- **KIQ:** How can I make a page look good on any screen?
- Colours, fonts, spacing, borders; draw the box model on paper before coding it
- Flexbox for rows and menus, Grid for card layouts, CSS variables for colours, one media query for phones
- **Mini-project:** Restyle the Week 1 profile, then build a responsive menu or price list for a local shop

### Week 3: JavaScript basics and the DOM

- **KIQ:** How can a page respond to what the user does?
- Variables, conditions, loops, and functions through small number and text games
- Select elements, listen for clicks, change text and colours
- **Mini-project:** A tip calculator or counter with a reset button

### Week 4: Modern JavaScript and tools (bridge week)

- **KIQ:** What do I need to know before React makes sense?
- Arrays, objects, map, filter, arrow functions, and destructuring on a list of products
- Git: init, commit, branch, push; start a Vite project; open DevTools and read error messages before asking for help
- **Mini-project:** A plain-JavaScript to-do list on GitHub, rebuilt in React in Week 6

### Week 5: Components, JSX, props and className

- **KIQ:** Why build pages from small reusable parts?
- Split a finished page into parts on paper first; write function components and JSX (one parent, closed tags, capitalised names)
- Pass props; show or hide parts with conditional rendering; style with className and one CSS file per component
- **Mini-project:** A product, student, or event card list from one Card component

### Week 6: State, events, lists and forms

- **KIQ:** How does a page remember and update information?
- useState for a counter, a toggle, and an input; lists with map and keys; a controlled form
- Lift state up so two components share one count, as in the React docs' two-button example
- **Mini-project:** The Week 4 to-do list rebuilt in React with add, delete, and mark-as-done; Session 3 is the CSS card workshop below

### Week 7: Effects and API data

- **KIQ:** How does my app get information from the internet?
- Explain an API with a restaurant-order analogy; read JSON in the browser
- One pattern only: fetch inside useEffect with loading and error messages and a search box
- Teacher demonstrates one simple Vitest test (not assessed)
- **Mini-project:** A weather, news, or country-facts app; Session 4 is the AI session below

### Week 8: Capstone and showcase

- **KIQ:** How do I plan, build, and share something useful?
- Day 1: idea, sketches, component list; Days 2 and 3: build with a daily teacher check-in; Day 4: publish, add to a one-page portfolio and GitHub profile, and present
- Peer feedback: two strengths and one suggestion
- **Capstone:** At least three components, one state, one list, and one form or API call, plus a README stating the problem, the solution, and one decision the learner made

## Styling in React with plain CSS (Week 6, Session 3)

Learners style one product card with a component CSS file, which is the same approach the [React Quick Start](https://react.dev/learn) shows: write the rules in a CSS file and attach them with className.

```jsx
import './Card.css';

export default function Card({ name, price, inStock }) {
  return (
    <div className="card">
      <h2 className="card-title">{name}</h2>
      <p className="card-price">KES {price}</p>
      <span className={inStock ? 'badge' : 'badge badge-out'}>
        {inStock ? 'In stock' : 'Sold out'}
      </span>
    </div>
  );
}
```

```css
:root { --green-bg: #dcfce7; --green-text: #166534; --red-bg: #fee2e2; --red-text: #991b1b; }
.card { padding: 16px; border: 1px solid #ddd; border-radius: 12px; max-width: 260px; }
.card-title { font-size: 1.125rem; margin: 0 0 8px; }
.card-price { color: #555; margin: 0 0 12px; }
.badge { background: var(--green-bg); color: var(--green-text); padding: 2px 10px; border-radius: 999px; font-size: 0.875rem; }
.badge-out { background: var(--red-bg); color: var(--red-text); }
```

**Session plan (3 hours).** 30 minutes: demo the finished card. 75 minutes: build it from a sketch. 45 minutes: make a Grid of six cards that becomes one column on phones. 30 minutes: debrief.

**Class naming rules for beginners**

- Start every class with the component name (card, card-title) so rules do not clash between components
- One CSS file per component, imported at the top of that component
- Put shared colours and spacing in CSS variables on :root
- Use classes, not ids, and avoid inline style unless a value comes from JavaScript
- When a style does not apply, open DevTools, click the element, and check which rule wins

## Session: build the feature, then improve the UI with AI (Week 7, Session 4)

Learners finish their own API app by hand, then use an AI assistant to improve only its look. The learner writes the logic, the AI suggests the styling, and the learner must be able to explain every line they keep.

| Part | Time | What learners do | Output |
| --- | --- | --- | --- |
| 1. Finish the technical build | 75 min | Complete the search box, loading message, and error message; test with bad input and no internet | Working plain app, committed as "working, unstyled" |
| 2. Improve the UI with AI | 75 min | Work on a new Git branch called ui-polish, one change at a time | Styled app and a before and after screenshot |
| 3. Review and reflect | 30 min | Keep or reject each change; write three sentences in the README | Merged or discarded branch |

```text
I am a beginner learning React. Here is my weather app component, my App.css,
and a screenshot.
Goal: make the UI cleaner and easier to read on a phone.
Rules: do not change any state, props, or fetch logic. Only change the JSX
structure and the CSS. Use plain CSS in App.css with CSS variables, no libraries.
Keep text readable, add alt text and form labels.
Give me the changed code and explain each change in one sentence.
```

**Review list**

- Search, loading, and error messages work exactly as before
- The learner can explain every line kept; anything unexplained is removed
- No new libraries were added and no logic was changed, otherwise the change is rejected
- The 5-point accessibility checklist passes: image alt text, form labels, readable contrast, keyboard use, heading order
- At least one design choice, such as colours or spacing, was made by the learner

**Ground rules.** Never paste passwords or API keys into an assistant. AI suggestions can be wrong, so run everything. Note "UI refined with AI assistance" in the README. Use a free chat assistant, or a local model through Ollama if data costs are a concern.

## Assessment and resources

Weekly mini-projects count for 60%, the capstone for 30%, and participation and peer review for 10%. Learners are rated on the KICD four-level scale: Exceeds (EE), Meets (ME), Approaches (AE), Below (BE).

| Competency | Meets expectations (ME) looks like | Exceeds (EE) adds |
| --- | --- | --- |
| HTML and CSS | A correct, readable, responsive page with Flexbox or Grid and CSS variables | Own design ideas and clean, reusable rules |
| JavaScript logic | Correct use of variables, conditions, loops, and functions | Solves new problems and explains the code |
| React components, props and state | Builds components; uses props, state, and lifted state correctly | Designs reusable components alone |
| Data and tools (API, Git, AI) | Fetches and shows data; pushes to GitHub; follows the AI prompt rules | Spots and fixes a problem the AI introduced |
| Communication and teamwork | Presents the work and gives feedback | Gives specific, kind feedback |

Learners rated AE or BE in a week get a short catch-up task next session. Capstone checks: runs without errors, three components, one state, one list, one form or API call, a published link, a README, a 3-minute demo, and the 5-point accessibility checklist.

### Links

| Topic | Link |
| --- | --- |
| React Quick Start and tutorial | [react.dev/learn](https://react.dev/learn) |
| HTML, CSS, JavaScript reference | [MDN Web Docs](https://developer.mozilla.org) |
| JavaScript explained simply | [javascript.info](https://javascript.info) |
| Free practice and certification path | [freeCodeCamp curriculum](https://learn.freecodecamp.org) |
| Editor, runtime, version control | [VS Code](https://code.visualstudio.com), [Node.js](https://nodejs.org), [Git](https://git-scm.com), [GitHub](https://github.com) |
| Project tool | [Vite](https://vite.dev) |
| Free hosting | [Netlify](https://www.netlify.com), [GitHub Pages](https://pages.github.com) |
| Contrast check for accessibility | [WebAIM contrast checker](https://webaim.org/resources/contrastchecker/) |
| Testing demo (Week 7) | [Vitest](https://vitest.dev) |
| Local AI model option | [Ollama](https://ollama.com) |

A Tailwind version of this course is in the [Tailwind track](beginner-with-tailwind.md).