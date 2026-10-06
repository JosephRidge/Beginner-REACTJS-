# React for Learners with JavaScript Background: Mid-Level Track (8 Weeks)

This 8-week KICD-style course is for learners who already know JavaScript and have only heard that React is a UI framework, and it moves quickly through the basics to TypeScript, testing, routing, data fetching, and a deployed capstone.

<!-- **Other tracks:** [Plain CSS track](../plain-css-track/README.md) · [Tailwind track](../tailwind-track/README.md) · [All tracks](../README.md) -->

## Contents

- [Course at a glance and strands](#course-at-a-glance-and-strands)
- [Week-by-week plan](#week-by-week-plan)
- [What finished code looks like](#what-finished-code-looks-like)
- [Build the feature, then improve the UI with AI](#session-build-the-feature-then-improve-the-ui-with-ai-week-5-session-4)
- [Assessment and resources](#assessment-and-resources)

## Course at a glance and strands

Learners cover the React Quick Start in one week, then spend the rest of the course on what separates a tutorial follower from a hireable junior: effects done right, data fetching, routing, TypeScript, testing, and a deployed project. Styling uses Tailwind for speed; learners who prefer plain CSS files can keep them, since styling is not assessed separately.

| Item | Detail |
| --- | --- |
| Duration | 8 weeks (assumed: 4 sessions a week, 3 hours each, about 96 hours) |
| Entry requirements | Comfortable with JavaScript functions, arrays, objects, async/await and fetch; HTML and CSS basics; Git add, commit, push |
| Entry check | A 60-minute Week 1 diagnostic: write a small JavaScript function set, fetch and show JSON in plain DOM code, and push to GitHub. Learners who struggle are advised to take the beginner track first |
| Approach | KICD competency-based and project-based; about 25% short talks, 75% hands-on, with weekly code review in pairs |
| Tools | VS Code, Vite, TypeScript, Tailwind, React Router, TanStack Query, Vitest and Testing Library, GitHub, Netlify |
| Exit outcome | Learner builds, tests, types, and deploys a multi-page React app and explains their decisions in a README and a short demo |

| Strand | Week | Sub-strand | Specific learning outcomes (by the end of the week the learner can…) |
| --- | --- | --- | --- |
| 1. React core | 1 | Components, JSX, props, state, events, lists, lifting state up | Rebuild a plain-JavaScript page as components; explain props versus state; share state between components |
| 2. State and effects | 2 | useState patterns, controlled forms, useEffect, derived data | Choose between state, derived values, and effects; clean up an effect; avoid effect loops and stale data |
| 3. Data and navigation | 3 | Fetching, loading and error states, TanStack Query, React Router | Fetch and cache server data; build a multi-page app with routes and URL parameters |
| 4. TypeScript | 4 | Types for props, state, events, and API data | Type components, hooks, and API responses; read and fix compiler errors |
| 5. Structure and reuse | 5 | Custom hooks, context, folder layout, Tailwind components | Extract a custom hook; share data with context where props get too deep; organise a project |
| 6. Quality | 6 | Testing, accessibility, linting, performance basics | Write component tests with Vitest and Testing Library; run an accessibility check; fix lint errors |
| 7. Full application | 7 | CRUD with an API, forms, environment variables, deployment pipeline | Build create, read, update, and delete screens; keep keys out of code; deploy automatically from GitHub |
| 8. Project and practice | 8 | Capstone, README, portfolio, interview practice | Deliver and explain a finished app and answer basic React questions aloud |

## Week-by-week plan

Each week has a key inquiry question (KIQ), hands-on experiences, and a deliverable pushed to GitHub. Session 1 is a short demo, Sessions 2 and 3 are build time with pair code review, and Session 4 is the deliverable and demo to peers.

### Week 1: React core in one week

- **KIQ:** What does React give me that plain JavaScript and the DOM did not?
- Day 1 diagnostic, then rebuild a plain-JavaScript to-do page as components so learners feel the difference
- Work through the [React Quick Start](https://react.dev/learn) and [Thinking in React](https://react.dev/learn/thinking-in-react): components, JSX rules, props, conditional rendering, lists with keys, events, useState, and lifting state up
- **Deliverable:** A product or student directory with search, built from at least four components

### Week 2: State and effects done properly

- **KIQ:** Which data belongs in state, which can be calculated, and when do I truly need an effect?
- Controlled forms, derived values instead of duplicated state, useReducer for a form with several fields
- useEffect: dependencies, cleanup, and why effects run twice in development; read [You Might Not Need an Effect](https://react.dev/learn/you-might-not-need-an-effect) and fix three given buggy components
- **Deliverable:** A multi-field form with validation, plus a short "bug fixes" list explaining each bug found

### Week 3: Data fetching and routing

- **KIQ:** How does an app get server data and show many pages without reloading?
- Hand-write a fetch with loading, error, and abort handling once, then replace it with TanStack Query and compare the code
- React Router: routes, links, URL parameters, a not-found page
- **Deliverable:** A three-page app (list, detail, search) using a public JSON API

### Week 4: TypeScript for React

- **KIQ:** How can the compiler catch my mistakes before the user does?
- Basic types, unions, optional values, interfaces versus type aliases; type props, useState, event handlers, and API responses
- Convert the Week 3 app to TypeScript one file at a time; learners read each compiler error aloud before fixing it
- **Deliverable:** The Week 3 app fully typed with no use of any, committed on a branch and merged by pull request

### Week 5: Structure, reuse and a UI pass

- **KIQ:** How do I keep a growing app readable?
- Custom hooks, context for shared data such as a theme or signed-in user, folder layout by feature
- Tailwind components: reuse by extracting components, not by copying class lists
- Session 4 is the build-then-improve-with-AI session described below
- **Deliverable:** The app refactored with at least one custom hook and one context, with a polished UI

### Week 6: Quality: tests, accessibility and linting

- **KIQ:** How do I know my app still works after I change it?
- Vitest and Testing Library: test what the user sees and does, not internal state; test a form, a list, and a failed fetch
- Accessibility: keyboard use, labels, contrast, heading order; run a browser accessibility audit and fix findings
- ESLint, and basic performance habits: avoid needless re-renders only after measuring
- **Deliverable:** At least six meaningful tests, a clean lint run, and a one-page accessibility report

### Week 7: A full application

- **KIQ:** How do create, read, update, and delete work end to end?
- Build CRUD screens against a small API (a local JSON Server or a free hosted backend); keep API keys in environment variables, never in code
- Basic sign-in concepts: tokens, protected routes, and why real security is checked on the server
- Deploy to Netlify or GitHub Pages directly from GitHub so every push updates the site
- **Deliverable:** CRUD app with routing, validation, loading and error states, and an automatic deployment

### Week 8: Capstone and job readiness

- **KIQ:** How do I show an employer what I can do?
- Day 1: plan, user stories, component and route map; Days 2 and 3: build with a daily check-in; Day 4: publish, demo, and peer review
- README states the problem, the solution, the tools, and three decisions made; add the project to a one-page portfolio and GitHub profile
- Mock technical interview: explain state versus props, why keys matter, what an effect cleanup does, and how a test was written
- **Capstone:** A typed, tested, deployed multi-page React app that fetches data, with a README and a three-minute demo

## What finished code looks like

By Week 6 learners should be able to write and explain code like this. In Week 3 they write the fetch by hand, and in Week 4 they type it; later they replace it with TanStack Query and compare.

```tsx
import { useEffect, useState } from 'react';

type Product = { id: number; name: string; price: number };

export function useProducts(search: string) {
  const [products, setProducts] = useState<Product[]>([]);
  const [loading, setLoading] = useState(true);
  const [error, setError] = useState<string | null>(null);

  useEffect(() => {
    const controller = new AbortController();

    async function load() {
      setLoading(true);
      setError(null);
      try {
        const res = await fetch(
          `/api/products?search=${encodeURIComponent(search)}`,
          { signal: controller.signal }
        );
        if (!res.ok) throw new Error(`Request failed: ${res.status}`);
        setProducts((await res.json()) as Product[]);
        setLoading(false);
      } catch (err) {
        if (controller.signal.aborted) return;
        setError(err instanceof Error ? err.message : 'Unknown error');
        setLoading(false);
      }
    }

    load();
    return () => controller.abort();
  }, [search]);

  return { products, loading, error };
}
```

Learners explain three things aloud: why the effect depends on search, why the cleanup aborts the old request, and why the early return on abort stops a stale response from changing the screen. The URL is a placeholder; point it at the course API.

A matching component test, using the counter from the [React Quick Start](https://react.dev/learn):

```tsx
import { render, screen } from '@testing-library/react';
import userEvent from '@testing-library/user-event';
import { expect, test } from 'vitest';
import MyButton from './MyButton';

test('counts clicks', async () => {
  render(<MyButton />);
  await userEvent.click(screen.getByRole('button', { name: /clicked 0 times/i }));
  expect(screen.getByRole('button', { name: /clicked 1 times/i })).toBeDefined();
});
```

This test assumes the component keeps its own count state and shows the text "Clicked 0 times", and Vitest needs a browser-like test environment such as jsdom, which the teacher sets up once in the starter project.

**Habits that signal a mid-level learner**

- Reads the error message and the docs before asking for help
- Keeps components small and names things by what they do
- Writes the loading and error states first, not last
- Tests behaviour a user can see, not internal details
- Commits small, with messages that say why

## Session: build the feature, then improve the UI with AI (Week 5, Session 4)

Learners first finish a feature by hand, then use an AI assistant for two jobs: polishing the UI, and reviewing their code. Employer guides list using AI assistants well, and checking their output critically, as a junior skill, so the session trains the checking as much as the prompting. The rule is that the learner writes the logic and must be able to explain every line they keep.

| Part | Time | What learners do | Output |
| --- | --- | --- | --- |
| 1. Technical build | 60 min | Extract the fetch logic into a custom hook, add a filter and a sort, and handle loading and error states | Working feature committed as "working, basic UI" |
| 2. Improve the UI with AI | 60 min | On a new branch ui-polish, give the assistant the component, a screenshot, and strict rules; apply one change at a time | Polished UI and before and after screenshots |
| 3. AI as reviewer | 40 min | Ask the assistant to list possible bugs and accessibility problems; verify each claim by testing or reading the docs | A table of claims marked true, false, or unsure |
| 4. Reflect | 20 min | Keep or reject each change; write three sentences in the README | Merged or discarded branch |

```text
I am learning React with TypeScript and Tailwind CSS v4. Here is my ProductList
component, my useProducts hook, and a screenshot.
Goal: make the UI cleaner and easier to scan on a phone.
Rules: do not change the hook, the types, state, or props. Only change JSX
structure and Tailwind classes. No new libraries. Keep it accessible: labels,
alt text, focus styles, and contrast.
Explain each change in one sentence and say what could go wrong with it.
```

```text
Review this component for bugs, stale-data problems in the effect, missing
loading or error handling, and accessibility issues. List each finding with the
line it refers to and how I can test whether it is real.
```

**Review list**

- The feature behaves exactly as before: filter, sort, loading, and error states
- The learner can explain every line kept; anything unexplained is removed
- No logic, types, or libraries were changed by the assistant
- At least one reviewer claim was shown to be wrong, with evidence
- The accessibility checklist passes: image alt text, form labels, readable contrast, keyboard use, heading order
- At least one design choice was made by the learner

**Ground rules.** Never paste passwords, tokens, or API keys into an assistant. Assistants can suggest outdated APIs or Tailwind v3 syntax, so check against the official docs and run everything. Note "UI refined with AI assistance" in the README. Use a free chat assistant, or a local model through Ollama if data costs are a concern. In Week 6 the same method applies to tests: the assistant may draft them, but the learner must make each test fail first by breaking the code, to prove it checks something.

## Assessment and resources

Weekly deliverables count for 50%, the capstone for 35%, and code review, participation, and the mock interview for 15%. Learners are rated on the KICD four-level scale: Exceeds (EE), Meets (ME), Approaches (AE), Below (BE).

| Competency | Meets expectations (ME) looks like | Exceeds (EE) adds |
| --- | --- | --- |
| React components, props and state | Splits a page into sensible components; places state correctly and lifts it when needed | Designs reusable components with clear interfaces |
| Effects and data | Fetches with loading, error, and cleanup handled; uses routing and URL parameters | Replaces hand-written fetching with TanStack Query and explains the trade-offs |
| TypeScript | Types props, state, events, and API data without any | Uses unions and generics to make wrong states impossible |
| Testing and quality | Six meaningful tests, clean lint run, accessibility audit fixed | Tests failure paths and shows each test fails when the code is broken |
| Full application and delivery | CRUD app deployed automatically from GitHub with keys kept out of code | Adds protected routes and clear error recovery |
| AI use and communication | Follows the prompt rules, checks AI claims, explains decisions in the README and demo | Finds and fixes a problem the AI introduced and explains why |

Learners rated AE or BE in a week get a short catch-up task, and a learner who is rated BE in two core areas by Week 3 is advised to repeat the beginner track.

### Links

| Topic | Link |
| --- | --- |
| React Quick Start | [react.dev/learn](https://react.dev/learn) |
| Thinking in React | [react.dev/learn/thinking-in-react](https://react.dev/learn/thinking-in-react) |
| Effects guidance | [You Might Not Need an Effect](https://react.dev/learn/you-might-not-need-an-effect) |
| React with TypeScript | [react.dev/learn/typescript](https://react.dev/learn/typescript) |
| TypeScript docs | [typescriptlang.org/docs](https://www.typescriptlang.org/docs/) |
| Routing | [React Router](https://reactrouter.com) |
| Server data | [TanStack Query](https://tanstack.com/query/latest) |
| Testing | [Vitest](https://vitest.dev), [Testing Library for React](https://testing-library.com/docs/react-testing-library/intro/) |
| Linting | [ESLint](https://eslint.org) |
| Tailwind installation with Vite | [tailwindcss.com/docs/installation/using-vite](https://tailwindcss.com/docs/installation/using-vite) |
| Next-step course for this level | [Full Stack Open (University of Helsinki)](https://fullstackopen.com/en/) |
| Free practice and certification path | [freeCodeCamp curriculum](https://learn.freecodecamp.org) |
| Reference and JavaScript review | [MDN Web Docs](https://developer.mozilla.org), [javascript.info](https://javascript.info) |
| Project tool | [Vite](https://vite.dev) |
| Free hosting | [Netlify](https://www.netlify.com), [GitHub Pages](https://pages.github.com) |
| Contrast check | [WebAIM contrast checker](https://webaim.org/resources/contrastchecker/) |
| Local AI model option | [Ollama](https://ollama.com) |

Full Stack Open is suggested as the follow-on because a 2026 course roundup describes it as using Vite, Vitest, and React Query and assuming basic JavaScript knowledge. Beginners should start with the other two tracks.