# POLAR-X Expedition Command

POLAR-X is a futuristic Antarctic expedition command-center platform for monitoring missions, cargo, inventory, personnel, assets, weather, alerts, and emergency operations from one interface.

The project is currently powered by realistic interconnected mock data and is designed as a polished frontend prototype for live demonstrations and future backend integration.

## What We Built

### Product Experience

- Premium blue and white mission-control interface
- Responsive desktop, laptop, tablet, and mobile layouts
- Shared sidebar navigation and top command header
- Interactive Antarctic live-view map treatment with stations, routes, transport, cargo, and personnel markers
- Mission performance charts using Recharts
- Consistent cards, status badges, alerts, timelines, tables, and operational panels
- Landing page for the POLAR-X product
- Secure-looking login experience for expedition administrators

### Current Routes

| Route | Purpose |
| --- | --- |
| `/` | POLAR-X landing page |
| `/login` | Expedition command login screen |
| `/dashboard` | Mission overview and command center |
| `/mission-map` | Live mission map and Bharati Station details |
| `/expeditions` | Expedition operations view |
| `/cargo` | Cargo shipments, filters, progress, and summary |
| `/inventory` | Inventory levels, fuel forecast, distribution, and status |
| `/personnel` | Personnel safety and assignment table |
| `/assets` | Vehicle, generator, and helicopter health monitoring |
| `/ai-intelligence` | Risk score, predictions, and AI insight signals |
| `/emergency` | Emergency response map and incident panel |
| `/analytics` | Mission analytics charts and performance data |

### Interactive Features

- React Router navigation with active sidebar states
- Responsive sidebar drawer on smaller screens
- Cargo tabs for All Cargo, In Transit, Delivered, and Delayed shipments
- Cargo search field and shipment progress indicators
- Add Cargo modal with form inputs
- Add Personnel modal with form inputs
- Mission and station action buttons
- Chart tooltips and responsive chart containers
- Map layer controls
- Alert and status visual states
- Login and logout navigation flow

## Technology Stack

- React
- TypeScript
- Vite
- React Router
- Lucide React
- Recharts
- Framer Motion dependency for future motion work
- Leaflet and React Leaflet dependencies for future live-map integration
- Responsive CSS with reusable design tokens

## Run Locally

```powershell
npm install
npm run dev
```

Open `http://localhost:5173` in your browser.

## Production Build

```powershell
npm run build
```

The production output is generated in the `dist` directory.

## Project Structure

```text
src/
  App.tsx       Main routes, shared components, mock data, and page views
  App.css       POLAR-X design system and responsive page styling
  index.css     Global browser and typography reset
  main.tsx      React application entry point
```

The current prototype keeps the main experience in `App.tsx` to make the demonstration easy to run. As the data model grows, the next refactor will move shared components and mock data into dedicated modules.

## What We Plan To Build Next

### Data and Backend

- Replace mock data with a typed API layer
- Add authentication and role-based access control
- Persist missions, cargo, personnel, assets, and alerts in a backend database
- Add real-time updates through WebSockets or server-sent events
- Add audit logs for operational changes

### Mission Operations

- Create a dedicated expedition-management workspace
- Add full mission creation and editing with validation
- Connect missions to assigned cargo, personnel, assets, risk, and activity history
- Add mission timeline editing and milestone tracking
- Add expedition comparison and mission performance reporting

### AI Assistant

- Add a floating AI command assistant available across the application
- Support natural-language queries over missions, cargo, threats, alerts, personnel, and network events
- Add suggested prompts, typing states, timestamps, and conversation history
- Connect the assistant to a secure model or local retrieval layer
- Add explainable recommendations and source records for AI answers

### Maps and Monitoring

- Replace the prototype map treatment with Leaflet map layers
- Add live station, vessel, aircraft, cargo, and personnel coordinates
- Add selectable station and asset detail panels
- Add weather, communication, emergency, and route overlays
- Add geofencing and location-based alerts

### Product Quality

- Add automated component and interaction tests
- Add end-to-end route and workflow tests
- Add loading, empty, error, and offline states
- Add accessibility review and keyboard navigation
- Improve code splitting for chart-heavy routes
- Add production monitoring and error reporting

## Current Status

POLAR-X is a functional frontend prototype with a complete visual system, multiple operational routes, responsive behavior, charts, mock map views, and interactive controls. The next major milestone is separating the data model from the UI and connecting the command center to a real backend and AI service.
