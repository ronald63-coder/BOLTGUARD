# BoltGuard

BoltGuard is a prototype dashboard exploring how vehicle monitoring could help identify conditions associated with brake failure before they contribute to road accidents. The current demo visualizes simulated sensor readings and maintenance signals; it is not connected to vehicle hardware and must not be used to make real-world safety decisions.

## Demo features

- Simulated vibration telemetry for sensors across several vehicles
- Status thresholds, alerts, and diagnostic summaries
- Vehicle and sensor views, with a rule-based risk analysis
- Responsive dashboard with light and dark themes

All readings and analysis are generated in the browser. The “AI” analysis is a local heuristic demonstration, not a validated predictive model. Brake-specific sensors, verified failure criteria, and real vehicle data integrations are not yet implemented.

## Run locally

The app is static and has no build step or package dependencies. Serve the repository root with any static HTTP server, then open the local address:

```powershell
python -m http.server 8000
```

Visit `http://localhost:8000`. The root `index.html` forwards to `BoltGuard.html`.

## Deployment

Deploy the repository root as a static site (for example, with Vercel). No build command or output directory is required. The root `index.html` forwards visitors to the dashboard.

## Safety note

This project is a software prototype, not a certified automotive safety system. Its simulated data, thresholds, and recommendations are illustrative only. Do not rely on them to diagnose, repair, or operate a vehicle.
