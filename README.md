# 🧠 Frontend Engineer Interview Q&A (Mid-Level)

---

## 🟨 JavaScript Core Concepts

### Q1: What is the difference between `var`, `let`, and `const`?
**A:**  
- `var`: Function-scoped, hoisted, can be redeclared.  
- `let`: Block-scoped, cannot be redeclared.  
- `const`: Same as `let`, but cannot be reassigned.

---

### Q2: What is a closure in JavaScript?
**A:**  
A closure is a function that captures variables from its lexical scope even after the outer function has returned.

---

### Q3: What is event delegation?
**A:**  
Attaching a single event listener to a parent element to manage events for its child elements using event bubbling.

---

### Q4: Explain prototypal inheritance.
**A:**  
JavaScript uses prototypes to allow objects to inherit properties and methods from other objects.

---

### Q5: What is the difference between `==` and `===`?
**A:**  
- `==`: Loose equality with type coercion.  
- `===`: Strict equality without type coercion.

---

### Q6: What is the event loop?
**A:**  
It enables non-blocking I/O by offloading operations to the browser’s APIs and queueing callbacks for execution.

---

### Q7: What are promises and async/await?
**A:**  
Promises represent the eventual result of an async operation.  
`async/await` is syntax sugar over promises for more readable code.

---

### Q8: What are arrow functions and how do they differ?
**A:**  
They are shorter functions that do **not bind** their own `this`, `arguments`, or `super`.

---

## ⚛️ React Core Concepts

### Q9: What is JSX?
**A:**  
JSX is a syntax extension that allows writing HTML inside JavaScript, transpiled to `React.createElement()`.

---

### Q10: What is the virtual DOM?
**A:**  
A lightweight representation of the real DOM used by React to optimize rendering.

---

### Q11: Explain `useState` and `useEffect`.
**A:**  
- `useState` manages local state in function components.  
- `useEffect` performs side-effects (like API calls) in components.

---

### Q12: What is the Context API?
**A:**  
Used for passing global data through the component tree without prop drilling.

---

### Q13: Difference between controlled and uncontrolled components?
**A:**  
- Controlled: Form input managed by React state.  
- Uncontrolled: Managed by the DOM using refs.

---

### Q14: What is reconciliation?
**A:**  
React’s process of comparing new virtual DOM with the old one and updating only what's changed.

---

### Q15: Explain `useMemo` and `useCallback`.
**A:**  
- `useMemo`: Memoizes expensive computations.  
- `useCallback`: Memoizes function references.

---

### Q16: What is `useReducer` used for?
**A:**  
Manages complex state logic similar to Redux but locally within a component.

---

### Q17: What is React Suspense?
**A:**  
A mechanism for handling async operations like code-splitting or data fetching with fallback UI.

---

## 🚀 Next.js Core Concepts

### Q18: What is file-based routing in Next.js?
**A:**  
Each file in the `pages/` directory corresponds to a route automatically.

---

### Q19: What are `getStaticProps`, `getServerSideProps`, `getInitialProps`?
**A:**  
- `getStaticProps`: Static generation.  
- `getServerSideProps`: Server-side rendering.  
- `getInitialProps`: Legacy data fetching method.

---

### Q20: What is ISR (Incremental Static Regeneration)?
**A:**  
Update static pages after deployment using `revalidate` property in `getStaticProps`.

---

### Q21: What are dynamic routes in Next.js?
**A:**  
Defined using square brackets, e.g. `[slug].js`, accessed via `useRouter()` or context.

---

### Q22: What is middleware in Next.js?
**A:**  
Runs before rendering to handle auth, redirects, or headers.

---

### Q23: How does Next.js optimize images?
**A:**  
Using `next/image` which offers built-in lazy loading, resizing, and WebP support.

---

### Q24: What are API routes in Next.js?
**A:**  
Built-in backend functions under `pages/api/`.

---

## 🔐 Authentication & Authorization

### Q25: What is JWT and how is it used?
**A:**  
JWT is a token-based authentication mechanism storing claims.  
Used to authorize user sessions via headers or cookies.

---

### Q26: What's the difference between authentication and authorization?
**A:**  
- Authentication: Verifying identity (login).  
- Authorization: Verifying access permissions.

---

### Q27: How do you implement protected routes?
**A:**  
- Frontend: Use auth context + route guards.  
- Backend: Check JWT/session token before responding.

---

## 🔧 API Communication

### Q28: How do you handle API calls in React?
**A:**  
Use `fetch`, `axios`, or `React Query` inside `useEffect` or custom hooks.

---

### Q29: What is optimistic UI update?
**A:**  
UI is updated immediately assuming the API call will succeed, and later corrected if it fails.

---

### Q30: What are some API status handling best practices?
**A:**  
- Show loaders  
- Handle error states  
- Retry logic  
- Success messages

---

## ⚙️ System Design + Coding Tasks

### Q31: Design a reusable Modal component in React.

### Q32: Design a front-end architecture for a video streaming platform.
- Components: Player, Playlist, Auth, Feed  
- Use: Lazy loading, code splitting, CDN caching  
- SEO: SSR with Next.js  
- Authentication: JWT + cookies

---

### Q33: Coding task  
> Build a dynamic table with sortable columns and pagination. Use `useState`, `useMemo`, and `useEffect`.

---

### Q34: How do you approach performance optimization?
**A:**  
- Use `React.memo`, `useMemo`, `useCallback`  
- Code-splitting  
- Image and font optimization  
- Lazy loading

---

## 🧩 Software Engineering Principles

### Q35: What are SOLID principles?
**A:**  
- S: Single Responsibility  
- O: Open/Closed  
- L: Liskov Substitution  
- I: Interface Segregation  
- D: Dependency Inversion

---

### Q36: What is DRY, KISS, and YAGNI?
**A:**  
- DRY: Don’t Repeat Yourself  
- KISS: Keep It Simple, Stupid  
- YAGNI: You Aren’t Gonna Need It

---

## 🎨 Design Patterns

### Q37: What is a Singleton Pattern?
**A:**  
A pattern that restricts a class to a single instance.

---

### Q38: What is a Higher Order Component (HOC)?
**A:**  
A function that takes a component and returns an enhanced component.

---

### Q39: Explain the Factory Pattern.
**A:**  
A method to create objects without specifying the exact class.

---

### Q40: What is the Observer Pattern in frontend?
**A:**  
Subscribers react to events from a subject (used in state management and event emitters).

---

## 🔁 Git, GitHub, and CI/CD

### Q41: How does `git rebase` differ from `git merge`?
**A:**  
- `merge`: Combines branches and creates a merge commit.  
- `rebase`: Rewrites history to apply commits linearly.

---

### Q42: What are common Git branching strategies?
**A:**  
- Git Flow  
- Trunk-based development  
- Feature branching

---

### Q43: What is a pull request and code review process?
**A:**  
A PR is a request to merge code; reviews ensure quality, style, and correctness.

---

### Q44: What are GitHub Actions?
**A:**  
CI/CD pipelines for testing, building, and deploying projects automatically.

---

### Q45: What is CI/CD?
**A:**  
- CI: Automatically testing code on every push.  
- CD: Automatically deploying code after CI passes.

---

### Q46: How do you write a good commit message?
**A:**  
- Use present tense: `Fix bug`, `Add login`  
- Follow conventional commits: `feat`, `fix`, `chore`, `refactor`, etc.

---
