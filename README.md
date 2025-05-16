# 🧠 Frontend Engineer Interview Q&A (Mid to Senior Level)

---

## 🟨 JavaScript Core Concepts

### 1. What is the difference between `var`, `let`, and `const`?  
**A:**  
- `var`: Function-scoped, hoisted, can be redeclared.  
- `let`: Block-scoped, not hoisted, cannot be redeclared but can be reassigned.  
- `const`: Block-scoped, not hoisted, cannot be redeclared or reassigned.

---

### 2. What is a closure in JavaScript?  
**A:**  
A closure is a function that retains access to its lexical scope even when the outer function has finished executing.

---

### 3. What is event delegation?  
**A:**  
Attaching a single event listener to a parent element to manage events from its child elements via event bubbling.

---

### 4. Explain prototypal inheritance.  
**A:**  
JavaScript objects inherit properties and methods from a prototype object, allowing shared functionality without classes.

---

### 5. What is the difference between `==` and `===`?  
**A:**  
- `==`: Loose equality with type coercion.  
- `===`: Strict equality without type coercion.

---

### 6. What is the event loop?  
**A:**  
It's a mechanism that handles asynchronous callbacks by processing the call stack and task queue to enable non-blocking I/O.

---

### 7. What are promises and async/await?  
**A:**  
Promises represent the result of async operations; `async/await` provides cleaner syntax to write asynchronous code using promises.

---

### 8. What are arrow functions and how do they differ?  
**A:**  
Arrow functions have a shorter syntax and do **not** have their own `this`, `arguments`, or `prototype`.

---

### 9. Explain "this" keyword in JavaScript.  
**A:**  
"this" references the object that is executing the current function, with its value determined by how the function is called.

---

### 10. What is the difference between call, apply, and bind?  
**A:**  
- `call`: Invokes a function with a specified this and individual arguments.
- `apply`: Invokes a function with a specified this and arguments as an array.
- `bind`: Returns a new function with a bound this and optional preset arguments.

---

### 11. Explain JavaScript's memory management and garbage collection.  
**A:**  
JavaScript automatically allocates memory when objects are created and frees it when they're no longer referenced. Garbage collection identifies and removes unreachable objects.

---

### 12. What are Web Workers?  
**A:**  
Background threads for executing scripts separate from the main thread, enabling concurrent processing without blocking the UI.

---

### 13. What is the difference between synchronous and asynchronous code?  
**A:**  
- Synchronous: Code executes sequentially, blocking until current operation completes.
- Asynchronous: Operations continue executing without waiting for long-running tasks to complete.

---

## ⚛️ React Core Concepts

### 14. What is JSX?  
**A:**  
JSX is a syntax extension for JavaScript that looks like HTML and transpiles to `React.createElement()` calls.

---

### 15. What is the virtual DOM?  
**A:**  
An in-memory representation of the real DOM that React uses to batch and optimize updates.

---

### 16. Explain `useState` and `useEffect`.  
**A:**  
- `useState`: Hook to manage component state.  
- `useEffect`: Hook to perform side effects like data fetching or subscriptions.

---

### 17. What is the Context API?  
**A:**  
A way to pass data through the component tree without prop drilling.

---

### 18. Difference between controlled and uncontrolled components?  
**A:**  
- Controlled: Form inputs controlled by React state.  
- Uncontrolled: Inputs managed by the DOM, accessed via refs.

---

### 19. What is reconciliation?  
**A:**  
React's process to compare virtual DOM trees and efficiently update the real DOM.

---

### 20. Explain `useMemo` and `useCallback`.  
**A:**  
- `useMemo`: Memoizes values to avoid expensive recalculations.  
- `useCallback`: Memoizes functions to avoid unnecessary re-creations.

---

### 21. What is `useReducer` used for?  
**A:**  
For managing complex state logic or multiple related state variables within a component.

---

### 22. What is React Suspense?  
**A:**  
A feature to handle asynchronous loading with fallback UIs, often used with lazy loading components or data fetching.

---

### 23. What is React Server Components?  
**A:**  
A new paradigm allowing components to render on the server, reducing client-side JavaScript and improving performance.

---

### 24. Explain the useLayoutEffect hook.  
**A:**  
Similar to useEffect but fires synchronously after DOM mutations and before browser paint, useful for DOM measurements.

---

### 25. What is React's Strict Mode?  
**A:**  
A development-only mode that identifies potential problems by intentionally double-invoking functions and highlighting deprecated APIs.

---

### 26. How does React handle error boundaries?  
**A:**  
Error boundaries are components that catch JavaScript errors in their child component tree, log those errors, and display a fallback UI.

---

### 27. Explain the difference between React state and props.  
**A:**  
- State: Private internal data managed by the component itself.
- Props: External data passed to a component from its parent.

---

## 🚀 Next.js Core Concepts

### 28. What is file-based routing in Next.js?  
**A:**  
Pages inside the `pages/` directory automatically become routes.

---

### 29. What are `getStaticProps`, `getServerSideProps`, `getInitialProps`?  
**A:**  
- `getStaticProps`: Fetches data at build time (static generation).  
- `getServerSideProps`: Fetches data on each request (server-side rendering).  
- `getInitialProps`: Legacy method for fetching data.

---

### 30. What is ISR (Incremental Static Regeneration)?  
**A:**  
Allows static pages to be updated after build with a revalidation interval.

---

### 31. What are dynamic routes in Next.js?  
**A:**  
Routes created with brackets, e.g., `[id].js`, for dynamic URL parameters.

---

### 32. What is middleware in Next.js?  
**A:**  
Code that runs before a request is completed, useful for auth, redirects, headers.

---

### 33. How does Next.js optimize images?  
**A:**  
`next/image` automatically provides lazy loading, resizing, and WebP format support.

---

### 34. What are API routes in Next.js?  
**A:**  
Backend endpoints defined in `pages/api/` folder to handle requests.

---

### 35. What is the App Router in Next.js?  
**A:**  
A new routing system introduced in Next.js 13 that uses a file-system based router built on React Server Components.

---

### 36. What are route handlers in Next.js 13+?  
**A:**  
Server-side functions that handle HTTP requests in the app directory, replacing API routes from the pages directory.

---

### 37. Explain the differences between the app directory and pages directory.  
**A:**  
App directory supports React Server Components, shared layouts, intercepting routes, and nested routes, while pages directory uses the older pages router.

---

### 38. How does Next.js handle code splitting?  
**A:**  
Automatically splits code by pages, dynamically loads components, and supports dynamic imports for optimal performance.

---

## 🔐 Authentication & Authorization

### 39. What is JWT and how is it used?  
**A:**  
JSON Web Tokens are compact, URL-safe tokens used to represent claims for authentication and authorization, often stored client-side.

---

### 40. What's the difference between authentication and authorization?  
**A:**  
- Authentication: Verifying who the user is.  
- Authorization: Determining what the user is allowed to do.

---

### 41. How do you implement protected routes?  
**A:**  
Use authentication state/context on frontend to guard routes, and verify tokens (JWT/session) on backend APIs.

---

### 42. What are the security considerations for JWT storage?  
**A:**  
Store JWTs in HttpOnly cookies to prevent XSS attacks, implement proper expiration times, and use HTTPS.

---

### 43. What is OAuth and how does it work?  
**A:**  
An open standard authorization framework that enables third-party applications to access resources without exposing credentials.

---

### 44. Explain CSRF attacks and prevention methods.  
**A:**  
Cross-Site Request Forgery tricks users into performing unwanted actions; prevent using CSRF tokens, SameSite cookies, and custom headers.

---

## 🔧 API Communication

### 45. How do you handle API calls in React?  
**A:**  
Using `fetch`, `axios`, or data-fetching libraries inside `useEffect` or custom hooks.

---

### 46. What is optimistic UI update?  
**A:**  
Updating the UI immediately assuming API success, then reverting if the call fails.

---

### 47. What are some API status handling best practices?  
**A:**  
Show loaders, handle errors gracefully, provide retry options, and show success confirmations.

---

### 48. What is REST API and its principles?  
**A:**  
Representational State Transfer is an architectural style with stateless client-server communication, uniform interface, cacheable resources, and a layered system.

---

### 49. What is GraphQL and how does it differ from REST?  
**A:**  
A query language for APIs that allows clients to request exactly what they need, reducing over-fetching and under-fetching common in REST.

---

### 50. Explain how to handle API rate limiting in frontend applications.  
**A:**  
Implement request throttling, queuing, batch requests, and proper error handling with exponential backoff for retry logic.

---

### 51. What is the SWR or React Query library and why use it?  
**A:**  
Libraries for data fetching that provide caching, automatic revalidation, pagination, and optimistic updates with minimal boilerplate.

---

## ⚙️ System Design + Coding Tasks

### 52. Design a reusable Modal component in React.  
*(Expect discussion on portal usage, accessibility, backdrop, and animation.)*

---

### 53. Design a front-end architecture for a video streaming platform.  
*(Discuss modular components, code splitting, SSR, caching, auth, and error handling.)*

---

### 54. Coding task: Build a dynamic table with sortable columns and pagination.  
*(Use hooks like `useState`, `useMemo`, and lifecycle methods.)*

---

### 55. How do you approach performance optimization?  
**A:**  
Use memoization (`React.memo`, `useMemo`, `useCallback`), code splitting, lazy loading, image optimization, and reduce unnecessary renders.

---

### 56. Design a state management system for a complex application.  
**A:**  
Consider centralized stores (Redux, Zustand), context API, server state libraries, and potentially a hybrid approach based on data types.

---

### 57. How would you build an accessible autocomplete component?  
**A:**  
Follow ARIA patterns, implement keyboard navigation, provide screen reader announcements, and manage focus correctly.

---

### 58. Design a drag-and-drop interface for reordering items.  
**A:**  
Use HTML5 Drag & Drop API or libraries like react-dnd, handle keyboard alternatives, and provide accessible feedback.

---

## 🧩 Software Engineering Principles

### 59. What are SOLID principles?  
**A:**  
- Single Responsibility  
- Open/Closed  
- Liskov Substitution  
- Interface Segregation  
- Dependency Inversion

---

### 60. What is DRY, KISS, and YAGNI?  
**A:**  
- DRY: Don't Repeat Yourself  
- KISS: Keep It Simple, Stupid  
- YAGNI: You Aren't Gonna Need It

---

### 61. What is separation of concerns in frontend development?  
**A:**  
Dividing application into distinct sections (presentation, business logic, data access) to improve maintainability and scalability.

---

### 62. Explain the concept of pure functions.  
**A:**  
Functions that always return the same output given the same input and have no side effects, making code more predictable and testable.

---

## 🎨 Design Patterns

### 63. What is a Singleton Pattern?  
**A:**  
Ensures a class has only one instance.

---

### 64. What is a Higher Order Component (HOC)?  
**A:**  
A function that takes a component and returns a new enhanced component.

---

### 65. Explain the Factory Pattern.  
**A:**  
A method for creating objects without exposing instantiation logic to the client.

---

### 66. What is the Observer Pattern in frontend?  
**A:**  
Subscribers listen and react to events or state changes from a subject.

---

### 67. What is the Render Props pattern?  
**A:**  
A technique for sharing code between components using a prop whose value is a function.

---

### 68. Explain the Container/Presentational pattern.  
**A:**  
Separating data fetching and state management (containers) from rendering UI (presentational components).

---

### 69. What is the Compound Component pattern?  
**A:**  
Components that work together to form a cohesive API, giving flexibility in composition while maintaining shared state.

---

## 🔁 Git, GitHub, and CI/CD

### 70. How does `git rebase` differ from `git merge`?  
**A:**  
- `merge`: Combines branches creating a merge commit.  
- `rebase`: Rewrites commit history to create a linear history.

---

### 71. What are common Git branching strategies?  
**A:**  
Git Flow, Trunk-based development, Feature branching.

---

### 72. What is a pull request and code review process?  
**A:**  
A PR is a request to merge code; code review ensures code quality and standards.

---

### 73. What are GitHub Actions?  
**A:**  
CI/CD pipelines to automate testing, building, and deploying projects.

---

### 74. What is CI/CD?  
**A:**  
- Continuous Integration: Automated testing on every code change.  
- Continuous Delivery/Deployment: Automated deployment after passing tests.

---

### 75. How do you write a good commit message?  
**A:**  
Use present tense and follow conventional commit types: `feat:`, `fix:`, `chore:`, etc.

---

### 76. What is git bisect and when would you use it?  
**A:**  
A binary search tool to find which commit introduced a bug by marking commits as "good" or "bad".

---

### 77. How do you resolve merge conflicts?  
**A:**  
Manually edit conflict markers in affected files, choose which changes to keep, then commit the resolved version.

---

## 🧪 Testing

### 78. What are the different types of frontend tests?  
**A:**  
Unit tests, integration tests, component tests, end-to-end tests, and visual regression tests.

---

### 79. What is Test-Driven Development (TDD)?  
**A:**  
A development process where tests are written before implementing features, following the red-green-refactor cycle.

---

### 80. How do you test React components?  
**A:**  
Using libraries like Jest and React Testing Library to test rendering, user interactions, and component behavior.

---

### 81. What is mocking in tests and when is it useful?  
**A:**  
Creating substitutes for dependencies to isolate code, control test conditions, and simulate specific scenarios.

---

### 82. How do you test asynchronous code?  
**A:**  
Using async/await with test frameworks, waiting for promises to resolve, and mocking timers for predictable testing.

---

## 🎨 Tailwind CSS, ShadCN UI & Radix UI

### 83. What is Tailwind CSS and how does it differ from traditional CSS frameworks like Bootstrap?  
**A:**  
Tailwind is a utility-first CSS framework providing low-level utility classes instead of pre-designed components like Bootstrap.

---

### 84. What are the advantages of using Tailwind CSS?  
**A:**  
- Highly customizable  
- Reduces CSS bloat  
- Speeds up styling with utilities  
- Easy to create responsive designs

---

### 85. How do you customize Tailwind CSS (e.g., colors, spacing)?  
**A:**  
By editing the `tailwind.config.js` file to extend or override default theme values.

---

### 86. What is ShadCN UI and how does it relate to Radix UI?  
**A:**  
ShadCN UI is a collection of reusable components built on Radix UI primitives, styled with Tailwind CSS, and designed to be copied into projects rather than installed as a dependency.

---

### 87. What are the benefits of Radix UI's headless components?  
**A:**  
They provide accessibility, keyboard navigation, and proper ARIA attributes while allowing complete styling freedom.

---

### 88. How do you handle dark mode with Tailwind CSS?  
**A:**  
Using the built-in dark mode variant with either class or media strategy, enabling conditional styling based on theme.

---

## 📱 Responsive Design & Accessibility

### 89. What are the key principles of responsive web design?  
**A:**  
Fluid grids, flexible images, and media queries to create layouts that adapt to different screen sizes and devices.

---

### 90. What is mobile-first design?  
**A:**  
Starting design and development for mobile devices first, then progressively enhancing for larger screens.

---

### 91. What are WCAG guidelines?  
**A:**  
Web Content Accessibility Guidelines defining how to make web content more accessible to people with disabilities.

---

### 92. How do you make a website keyboard accessible?  
**A:**  
Ensure all interactive elements are focusable, provide visible focus indicators, and implement proper tab order.

---

### 93. What are ARIA roles and when should you use them?  
**A:**  
Accessible Rich Internet Applications roles help define element purposes for assistive technologies, used when HTML semantics aren't sufficient.

---

### 94. How do you test for accessibility?  
**A:**  
Use automated tools like Lighthouse, manual testing with screen readers, keyboard navigation testing, and following WCAG checklists.

---

## 📊 Performance Optimization

### 95. What is the Core Web Vitals and why are they important?  
**A:**  
Google's metrics for user experience: LCP (loading), FID (interactivity), and CLS (visual stability), which impact SEO and user experience.

---

### 96. How do you optimize website loading speed?  
**A:**  
Code splitting, lazy loading, image optimization, caching, minification, and reducing render-blocking resources.

---

### 97. What is tree shaking?  
**A:**  
A bundler optimization that removes unused code from the final bundle, reducing file size.

---

### 98. How do you diagnose performance issues?  
**A:**  
Using Chrome DevTools performance panel, Lighthouse audits, React Profiler, and monitoring real user metrics.

---

### 99. What is the difference between client-side and server-side rendering?  
**A:**  
- Client-side: Browser renders HTML using JavaScript after page load.
- Server-side: Server sends fully rendered HTML to browser, improving initial load time and SEO.

---

### 100. What is code splitting and why is it important?  
**A:**  
Breaking code into smaller chunks loaded on demand, improving initial load time by only loading what's needed.

---

## 🌐 Modern Frontend Development

### 101. What is a progressive web app (PWA)?  
**A:**  
Web applications that use modern web capabilities to provide app-like experiences with offline functionality, push notifications, and installability.

---

### 102. What is WebAssembly (WASM) and its use cases?  
**A:**  
A binary instruction format for executing high-performance code in web browsers, useful for CPU-intensive tasks like games, video editing, and encryption.

---

### 103. How do micro-frontends work?  
**A:**  
An architectural approach where a frontend is decomposed into semi-independent applications maintained by different teams.

---

### 104. What are Web Components?  
**A:**  
Custom, reusable, encapsulated HTML elements built using standard web platform APIs: Custom Elements, Shadow DOM, and HTML Templates.

---

### 105. What are the current trends in state management beyond Redux?  
**A:**  
Context API with useReducer, Zustand, Jotai, Recoil, and XState for simpler, more flexible state management solutions.

---
