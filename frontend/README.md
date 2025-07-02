# Frontend Deployment Instructions

- Place your static HTML, CSS, and JS files in this `frontend/` directory.
- Push this directory to your GitHub repository.
- In your repository settings, enable GitHub Pages and set the source to the `frontend/` folder (or the branch/folder you prefer).
- Update all API calls in your frontend code to use the full Vercel deployment URL, e.g.:
  ```
  fetch('https://your-vercel-app.vercel.app/api/create-session', {...})
  ```
- Do **not** use relative API URLs like `/api/create-session` in production, as the frontend and backend are on different domains.
