# Beginner Web Development with React: Tailwind Track (8 Weeks)

This 8-week KICD-style beginner course teaches CSS fundamentals in Week 2, then styles all React work with Tailwind CSS utility classes from Week 5 onward.

<!-- **Other tracks:** [Plain CSS track](../plain-css-track/README.md) · [Mid-level track](../mid-level-track/README.md) · [All tracks](../README.md) -->

## Contents

- [Course at a glance and strands](#course-at-a-glance-and-strands)
- [Week-by-week plan](#week-by-week-plan)
- [Styling in React with Tailwind](#styling-in-react-with-tailwind-setup-in-week-4-practice-from-week-5)
- [Build the feature, then improve the UI with AI](#session-build-the-feature-then-improve-the-ui-with-ai-week-7-session-4)
- [Assessment and resources](#assessment-and-resources)

## Course at a glance and strands

Learners spend four weeks on web basics, three on React, and one on a showcase project. Tailwind utilities are CSS in short form, so Week 2 still teaches core CSS, and Tailwind arrives with the Vite project in Week 4.

| Item | Detail |
| --- | --- |
| Duration | 8 weeks (assumed: 4 sessions a week, 3 hours each, about 96 hours) |
| Level | Absolute beginner; basic computer literacy and a laptop |
| Approach | KICD competency-based and project-based; about 30% short talks, 70% hands-on |
| Tools | VS Code, Chrome, Git and GitHub, Node.js with Vite, Tailwind CSS, Netlify or GitHub Pages |
| Styling | Core CSS in Weeks 1 to 3; Tailwind utility classes in Weeks 5 to 8 |
| Exit outcome | Learner builds, styles, and publishes a small React app and can explain what each utility class does in CSS |

| Strand | Week | Sub-strand | Specific learning outcomes (by the end of the week the learner can…) |
| --- | --- | --- | --- |
| 1. Web foundations | 1 | How the web works; HTML | Explain browser, server, and URL; build a page with headings, images, links, lists, and a form |
| 2. Styling and layout | 2 | Core CSS, Flexbox, responsive design | Style text, colour, and spacing; lay out content with Flexbox; explain the box model; make a page work on phone and laptop |
| 3. JavaScript | 3 | Core JavaScript; the DOM | Use variables, conditions, loops, and functions; react to clicks and change the page |
| 3. JavaScript | 4 | Modern JavaScript; Git; tools; Tailwind setup | Use arrays, map, filter, objects, arrow functions, and destructuring; commit, branch, and push with Git; start a Vite project and add Tailwind |
| 4. Building with React | 5 | Components, JSX, props, utility classes | Build reusable components; pass props; style with Tailwind classes in className; show content conditionally |
| 4. Building with React | 6 | State, events, lists, forms | Use useState; show lists with keys; build a controlled form; lift state up; use hover, focus, and responsive prefixes |
| 4. Building with React | 7 | Effects and API data | Load data with useEffect and fetch; show loading and error messages; refine the UI with AI safely |
| 5. Project and practice | 8 | Capstone and deployment | Plan, build, publish, and present a React app with a README and a portfolio page |

## Week-by-week plan

Each week has a key inquiry question (KIQ), hands-on experiences, and a mini-project pushed to GitHub. Session 1 is a demo, Sessions 2 and 3 are guided pair practice, and Session 4 is the mini-project and peer review.

### Week 1: How the web works and HTML

- **KIQ:** What happens when I type a web address and press Enter?
- Role-play browser, server, and request; use "View Source" on a school or news site
- Build a profile page with headings, a photo with alt text, a list, links, and a contact form
- **Mini-project:** A one-page profile for the learner or a local group

### Week 2: Core CSS and responsive design

- **KIQ:** How can I make a page look good on any screen?
- Colours, fonts, spacing, borders; draw the box model on paper before coding it
- Flexbox for rows and menus, one media query for phones; keep a "CSS cheat card" of property names (padding, margin, border-radius, flex, gap), which becomes the key to reading Tailwind later
- **Mini-project:** Restyle the Week 1 profile, then build a responsive menu or price list for a local shop

### Week 3: JavaScript basics and the DOM

- **KIQ:** How can a page respond to what the user does?
- Variables, conditions, loops, and functions through small number and text games
- Select elements, listen for clicks, change text and colours
- **Mini-project:** A tip calculator or counter with a reset button

### Week 4: Modern JavaScript, Git and Tailwind setup (bridge week)

- **KIQ:** What do I need to know before React makes sense?
- Arrays, objects, map, filter, arrow functions, and destructuring on a list of products
- Git: init, commit, branch, push; start a Vite project and add Tailwind with the steps in the next section; open DevTools and read error messages before asking for help
- Play with the [Tailwind Play](https://play.tailwindcss.com) editor: change one class at a time and match each class to the CSS shown
- **Mini-project:** A plain-JavaScript to-do list on GitHub, rebuilt in React in Week 6

### Week 5: Components, JSX, props and utility classes

- **KIQ:** Why build pages from small reusable parts?
- Split a finished page into parts on paper first; write function components and JSX (one parent, closed tags, capitalised names)
- Pass props; show or hide parts with conditional rendering; style with Tailwind classes in className and look classes up in the docs search
- Rule: when a className gets long, make it a component, not a copy-paste
- **Mini-project:** A product, student, or event card list from one Card component

### Week 6: State, events, lists and forms

- **KIQ:** How does a page remember and update information?
- useState for a counter, a toggle, and an input; lists with map and keys; a controlled form
- Lift state up so two components share one count, as in the React docs' two-button example
- Style states with hover:, focus:, and md: prefixes on the form and buttons
- **Mini-project:** The Week 4 to-do list rebuilt in React with add, delete, and mark-as-done

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

## Styling in React with Tailwind (setup in Week 4, practice from Week 5)

Setup takes three steps in a Vite project (Tailwind v4; the teacher checks the [official Vite guide](https://tailwindcss.com/docs/installation/using-vite) on the day, since steps change between versions):

1. Run `npm install tailwindcss @tailwindcss/vite`.
2. In `vite.config.js`, import the plugin with `import tailwindcss from '@tailwindcss/vite'` and add `tailwindcss()` to the plugins list.
3. Put `@import "tailwindcss";` at the top of `src/index.css`.

Then the product card needs no CSS file; the styling sits in the className values.

```jsx
export default function Card({ name, price, inStock }) {
  const badge = inStock
    ? 'bg-green-100 text-green-800'
    : 'bg-red-100 text-red-800';

  return (
    <div className="max-w-[260px] rounded-xl border border-gray-300 p-4">
      <h2 className="mb-2 text-lg font-semibold">{name}</h2>
      <p className="mb-3 text-gray-600">KES {price}</p>
      <span className={`rounded-full px-2.5 py-0.5 text-sm ${badge}`}>
        {inStock ? 'In stock' : 'Sold out'}
      </span>
    </div>
  );
}
```

**Reading Tailwind (Week 5 activity).** Learners translate each class back to CSS using the Week 2 cheat card: p-4 is padding of 1rem, rounded-xl is a large border-radius, text-lg is a larger font size, mb-2 is a bottom margin. A learner who can do this can debug Tailwind, because the classes are CSS in short form.

**Habits for beginners**

- Write full class names such as bg-green-100, never build a class name by joining text pieces, because Tailwind only creates the classes it can see written out
- Keep one component per file so long className lists stay small
- Use the docs search box for every class you do not know, and add the CSS meaning to your cheat card
- When a layout looks wrong, check DevTools to see which classes are applied
- Weeks 1 to 3 stay Tailwind-free so learners know what the classes stand for

## Session: build the feature, then improve the UI with AI (Week 7, Session 4)

Learners finish their own API app by hand, then use an AI assistant to improve only its look with Tailwind classes. The learner writes the logic, the AI suggests the styling, and the learner must be able to say what each class means in CSS.

| Part | Time | What learners do | Output |
| --- | --- | --- | --- |
| 1. Finish the technical build | 75 min | Complete the search box, loading message, and error message; test with bad input and no internet | Working app with basic Tailwind styling, committed as "working, basic UI" |
| 2. Improve the UI with AI | 75 min | Work on a new Git branch called ui-polish, one change at a time | Polished app and a before and after screenshot |
| 3. Review and reflect | 30 min | Keep or reject each change; write three sentences in the README | Merged or discarded branch |

```text
I am a beginner learning React with Tailwind CSS v4 on Vite. Here is my weather
app component and a screenshot.
Goal: make the UI cleaner and easier to read on a phone.
Rules: do not change any state, props, or fetch logic. Only change the JSX
structure and Tailwind classes. Use full class names, no plugins, no extra
libraries. Keep text readable, add alt text and form labels.
Give me the changed code and explain what each new class does in plain CSS.
```

**Review list**

- Search, loading, and error messages work exactly as before
- The learner can state the CSS meaning of every new class kept; anything unexplained is removed
- No new libraries or plugins were added and no logic was changed, otherwise the change is rejected
- The class list is not copied three times; repeated blocks become a component
- The 5-point accessibility checklist passes: image alt text, form labels, readable contrast, keyboard use, heading order
- At least one design choice, such as colours or spacing, was made by the learner

**Ground rules.** Never paste passwords or API keys into an assistant. AI suggestions can be wrong, and assistants sometimes use older Tailwind v3 setup or class names, so check against the docs and run everything. Note "UI refined with AI assistance" in the README. Use a free chat assistant, or a local model through Ollama if data costs are a concern.

## Assessment and resources

Weekly mini-projects count for 60%, the capstone for 30%, and participation and peer review for 10%. Learners are rated on the KICD four-level scale: Exceeds (EE), Meets (ME), Approaches (AE), Below (BE).

| Competency | Meets expectations (ME) looks like | Exceeds (EE) adds |
| --- | --- | --- |
| HTML and core CSS | A correct, readable, responsive page with Flexbox and the box model explained | Own design ideas and clean structure |
| JavaScript logic | Correct use of variables, conditions, loops, and functions | Solves new problems and explains the code |
| React components, props and state | Builds components; uses props, state, and lifted state correctly | Designs reusable components alone |
| Tailwind styling | Styles components with utility classes and states the CSS meaning of common classes | Extracts repeated class lists into components and fixes layout bugs from DevTools |
| Data and tools (API, Git, AI) | Fetches and shows data; pushes to GitHub; follows the AI prompt rules | Spots and fixes a problem the AI introduced |
| Communication and teamwork | Presents the work and gives feedback | Gives specific, kind feedback |

Learners rated AE or BE in a week get a short catch-up task next session. Capstone checks: runs without errors, three components, one state, one list, one form or API call, a published link, a README, a 3-minute demo, and the 5-point accessibility checklist.

### Links

| Topic | Link |
| --- | --- |
| React Quick Start and tutorial | [react.dev/learn](https://react.dev/learn) |
| Tailwind installation with Vite | [tailwindcss.com/docs/installation/using-vite](https://tailwindcss.com/docs/installation/using-vite) |
| Tailwind docs and class search | [tailwindcss.com/docs](https://tailwindcss.com/docs) |
| Try Tailwind in the browser | [Tailwind Play](https://play.tailwindcss.com) |
| HTML, CSS, JavaScript reference | [MDN Web Docs](https://developer.mozilla.org) |
| JavaScript explained simply | [javascript.info](https://javascript.info) |
| Free practice and certification path | [freeCodeCamp curriculum](https://learn.freecodecamp.org) |
| Editor, runtime, version control | [VS Code](https://code.visualstudio.com), [Node.js](https://nodejs.org), [Git](https://git-scm.com), [GitHub](https://github.com) |
| Project tool | [Vite](https://vite.dev) |
| Free hosting | [Netlify](https://www.netlify.com), [GitHub Pages](https://pages.github.com) |
| Contrast check for accessibility | [WebAIM contrast checker](https://webaim.org/resources/contrastchecker/) |
| Testing demo (Week 7) | [Vitest](https://vitest.dev) |
| Local AI model option | [Ollama](https://ollama.com) |

A plain CSS version of this course is in the [Plain CSS track](beginner-with-plain-css.md).