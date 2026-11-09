# Tech Mind Dashboard

A React dashboard front end built with Material-UI. It currently contains the responsive top navigation bar (the app shell).

## Features

- Responsive app bar with a menu button, the "Tech Mind Dashboard" title and a search box
- Mail and notification icons with badge counters
- Profile menu (Profile, My account)
- Mobile layout: the icons collapse into a single "more" menu on small screens
- Accessible markup (ARIA labels on all icon buttons)

## Tech Stack

- [React](https://reactjs.org/) (bootstrapped with Create React App)
- [Material-UI v4](https://v4.mui.com/) (`@material-ui/core`, `@material-ui/icons`)
- Jest and React Testing Library for tests

## Project Structure

```
src/
├── App.js                  # Main component: responsive search app bar
├── App.css / index.css     # Styles
├── index.js                # App entry point
├── components/
│   ├── login.js            # Login page (placeholder, empty)
│   └── register.js         # Registration page (placeholder, empty)
├── App.test.js             # Default CRA test (needs updating)
├── reportWebVitals.js
└── setupTests.js
```

## Getting Started

This repository contains the `src` folder of a Create React App project. To run it:

```bash
# 1. Create a CRA project (skip if you already have a package.json)
npx create-react-app tech-mind-dashboard
cd tech-mind-dashboard

# 2. Install Material-UI v4
npm install @material-ui/core@4 @material-ui/icons@4

# 3. Replace the generated src/ folder with this repo's src/ folder, then:
npm start
```

The app opens at http://localhost:3000.

### Scripts

| Command         | Description                      |
| --------------- | -------------------------------- |
| `npm start`     | Run the app in development mode  |
| `npm test`      | Run the tests                    |
| `npm run build` | Create a production build        |

## Roadmap

- [ ] Build the login and registration forms (`components/login.js`, `components/register.js`)
- [ ] Add routing (e.g. React Router) between pages
- [ ] Make search, mail and notifications work with real data (counters are currently hard-coded)
- [ ] Update `App.test.js`, which still checks for the default "learn react" text
- [ ] Add a `package.json` and the `public/` folder to the repo
