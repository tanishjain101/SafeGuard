# SafeGuard

SafeGuard is a React + Vite emergency safety web app designed for quick response during critical situations.

It helps users:
- trigger SOS alerts,
- share live location with emergency contacts,
- access emergency numbers,
- view weather conditions/alerts,
- use offline-friendly emergency tools and planning guides.

## Highlights

- Emergency SOS flow with location support
- Quick emergency actions (call, location share, medical info, incident report, flashlight, radio)
- Weather widget with forecast and alert support
- Disaster planning and preparedness checklists
- Emergency contact management
- Multi-language UI support
- Offline support via service worker + local storage cache
- Emergency number updated to **112** in core call flows

## Tech Stack

- React 18
- TypeScript
- Vite
- Tailwind CSS
- ESLint

## Project Structure

```text
SafeGuard/
  src/
    components/
    services/
    App.tsx
    main.tsx
  public/
    sw.js
  index.html
  package.json
```

## Getting Started

### 1. Install dependencies

```bash
cd /Users/tanishjain/Desktop/project/SafeGuard
npm install
```

### 2. Run development server

```bash
npm run dev
```

The app is configured to run on:

- `http://127.0.0.1:5500/`

### 3. Build for production

```bash
npm run build
```

### 4. Preview production build locally

```bash
npm run preview
```

## Important: How to Open the App Correctly

Use the Vite dev server URL only.

- Correct: `http://127.0.0.1:5500/`
- Incorrect: opening `index.html` directly (`file://...`)
- Incorrect: serving with plain static "Live Server" while expecting `/src/main.tsx` to load as TS module

If opened the wrong way, browser may show:

- `Failed to fetch dynamically imported module`
- white/blank screen

## Troubleshooting

### White screen or startup error

1. Stop old servers:

```bash
pkill -f "vite|live-server|python -m http.server" || true
```

2. Start fresh:

```bash
npm run dev
```

3. Open exactly:

- `http://127.0.0.1:5500/`

4. Hard refresh browser (`Cmd+Shift+R` on macOS).

### Port already in use

The dev script uses `--strictPort`; it will fail instead of switching ports.

- free the port or stop old process, then rerun `npm run dev`.

## Available Scripts

- `npm run dev` - start Vite dev server on `127.0.0.1:5500`
- `npm run build` - production build into `dist/`
- `npm run preview` - preview built app
- `npm run lint` - run ESLint

## Deploying

Any static hosting works (Vercel, Netlify, Firebase Hosting, GitHub Pages with proper config).

Typical flow:

1. `npm run build`
2. Deploy `dist/` directory
3. Share the hosted `https://...` URL

## Emergency Numbers (Current App Defaults)

- Emergency Services: **112**
- Fire: 101
- Medical: 102
- Disaster Management: 108
- Women Helpline: 1091
- Child Helpline: 1098

## Safety Disclaimer

This app is an aid tool. In a real emergency, contact official emergency services immediately.

