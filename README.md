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

## Important: How to Open the App Correctly

1. Stop old servers:

```bash
pkill -f "vite|live-server|python -m http.server" || true
```

2. Start fresh:

```bash
npm run dev
```

## Deploying

Any static hosting works (Vercel, Netlify, Firebase Hosting, GitHub Pages with proper config).

Typical flow:


## Emergency Numbers (Current App Defaults)

- Emergency Services: **112**
- Fire: 101
- Medical: 102
- Disaster Management: 108
- Women Helpline: 1091
- Child Helpline: 1098

## Safety Disclaimer

This app is an aid tool. In a real emergency, contact official emergency services immediately.

