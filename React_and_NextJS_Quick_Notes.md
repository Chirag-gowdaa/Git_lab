# React & Next.js Quick Revision Notes

## React Basics
- Component-Based: UI is built from reusable components (functions or classes).
- JSX: Syntax extension that looks like HTML but is rendered by React.
- Props: Inputs to components; read-only.
- State: Data managed within a component, triggers re-render on change (via `useState` in function components).
- Lifecycle Methods: Functions called at specific points (e.g., `useEffect` for side-effects in function components).
- Events: Handled using event handlers like `onClick`, `onChange`.
- Lists & Keys: Render lists with `array.map()`, each child needs a unique `key`.

### Hooks
- `useState`: Manage state in function components.
- `useEffect`: Run side effects (like data fetching).
- `useContext`: Share state globally.
- `useRef`, `useMemo`, `useCallback`: For advanced scenarios.

### Conditional Rendering
```jsx
{isLoggedIn ? <LogoutButton /> : <LoginButton />}
```

### Forms
- Controlled inputs: value & onChange managed by state.

---

## Next.js Essentials
- File-based Routing: Pages are React components in the `/pages` or `/app` directory.
- Dynamic Routes: Use `[param].js` for dynamic segments.
- API Routes: Serverless functions in `/pages/api`.

### Data Fetching
- `getStaticProps`: Fetch data at build time (Static Site Generation - SSG).
- `getServerSideProps`: Fetch data at request time (Server Side Rendering - SSR).
- `getStaticPaths`: For dynamic SSG pages.
- In Next 13+, use `app/` directory with server components and `fetch()`. 

### Routing
- Use `next/link` for navigation (client-side).
- Use `useRouter` hook for programmatic navigation.

### Image Optimization
- Use `next/image` for optimized images.

### Built-in CSS Support
- Use global CSS (`pages/_app.js`) or module CSS (`Component.module.css`).
- Supports Sass, CSS-in-JS, Tailwind, etc.

### API Routes
- Create backend endpoints in `/pages/api/filename.js`.

### Deployment
- Vercel is the default platform, but Next.js can run anywhere Node.js runs.

---

## Tips
- React: Focus on component composition and hooks.
- Next.js: Leverage built-in routing and data-fetching for SEO and performance.
- Both: Use dev tools and error overlays for debugging.


## Useful Links
- React Docs: https://react.dev/
- Next.js Docs: https://nextjs.org/docs