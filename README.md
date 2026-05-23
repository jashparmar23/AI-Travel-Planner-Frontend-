# AI Travel Planner - Frontend Dashboard

A premium, state-of-the-art dark-mode glassmorphic user interface for the AI Travel Planner. This static single-page web app lets you visually interact with the multi-agent travel orchestrator backend, watch agent stages in real-time, and run the Human-in-the-Loop review and revision cycles.

## Key UI Features

- **Glassmorphic Design**: Sleek backdrop blurs, radial glowing filters, and vibrant neon gradients that match modern design criteria.
- **Dynamic Input tag builder**: Easily customize traveler sizes, budget ranges, and type in tag preferences with standard placeholders prefilled.
- **Dynamic State Timeline**: Tracks the LangGraph backend thread stages (`Submitted` -> `Researching` -> `Planning` -> `Reviewing` -> `Finalized`) dynamically via API polling.
- **Review Studio Panel**: Full day-by-day itinerary accordions displaying daily themes, activity schedulers, meal guidelines, lodging, guidelines, and packing recommendations.
- **HITL Integration**: Live Approve & Finalize, Reject with Comments, or Modify actions with client-side character validations to prevent empty submissions.
- **Decoupled API Settings Configuration**: Features a premium floating **Gear Icon Settings Panel** in the top-right corner to point the static site dynamically to local host endpoints (`http://localhost:8000`) or production APIs (like a live Render endpoint). Remembers configuration settings via `localStorage`.

---

## Quick Setup & Run

The frontend is a static web app. No bundlers or server-side installs are needed.

### 1. Locally

You can open the `index.html` file directly in any modern browser!

Alternatively, you can run a simple, lightweight server to serve the page:

```bash
# Python 3+
python -m http.server 3000
```
Then visit: `http://localhost:3000`

### 2. Configure Backend Server Endpoint

1. When the page loads, click the **Settings Gear Icon** at the top right of the page.
2. Enter your running FastAPI backend URL (e.g. `http://localhost:8000` or your Render backend URL `https://your-service.onrender.com`).
3. Click **Save Endpoint Settings**. It will be saved into your browser's local storage and used for all travel generations!

---

## Deployment

Since this repository is purely static files (`index.html`), it is extremely cheap and fast to deploy. You can host it instantly for free on:
- **Netlify**
- **Vercel**
- **GitHub Pages**
- **Render (Static Site)**
