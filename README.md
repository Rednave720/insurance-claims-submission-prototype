# Insurance Claims Submission Prototype

An early React + Firebase insurance claims prototype built to explore claim intake, NoSQL persistence, and user-facing submission workflows.

## Project Context

This project was created as an early insurance-technology prototype while preparing for AIG interview conversations. The goal was to quickly demonstrate claim intake, frontend form handling, and cloud database persistence using React and Firebase Realtime Database.

This project later informed a more advanced full-stack Insurance Claims Management Portal built with Spring Boot, PostgreSQL, React, REST APIs, Material UI, admin review workflows, status tracking, audit history, dashboard summaries, and document metadata.

## What This Prototype Demonstrates

- A simple claim intake form for name, email, policy number, and claim description
- Basic frontend form validation
- Firebase Realtime Database write/read interaction
- A claims list view showing submitted claim records
- Bootstrap-based responsive UI layout
- Early insurance-domain product thinking and initiative

## Tech Stack

- React
- Vite
- Firebase Realtime Database
- Bootstrap
- React Router

## Local Setup

Install dependencies:

```bash
npm install
```

Create a local `.env` file using `.env.example` as a template:

```bash
cp .env.example .env
```

Add your Firebase web app configuration values:

```text
VITE_FIREBASE_API_KEY=
VITE_FIREBASE_AUTH_DOMAIN=
VITE_FIREBASE_DATABASE_URL=
VITE_FIREBASE_PROJECT_ID=
VITE_FIREBASE_STORAGE_BUCKET=
VITE_FIREBASE_MESSAGING_SENDER_ID=
VITE_FIREBASE_APP_ID=
```

Run the app:

```bash
npm run dev
```

The app runs locally at:

```text
http://localhost:5173
```

## Validation Commands

```bash
npm run lint
npm run build
```

## Firebase Security Note

This app uses Firebase client-side configuration through Vite environment variables. Firebase web config values are not traditional server secrets, but the database must still be protected with appropriate Firebase Realtime Database rules.

Before using this project with a real Firebase project, confirm that:

- `.env` is not committed
- Realtime Database rules do not allow unrestricted public reads/writes
- The database only stores safe demo data
- No sensitive personal, financial, medical, or policy data is submitted

## MVP Limitations

- Prototype only, not a production insurance platform
- No authentication or role-based access control
- No admin review workflow
- No claim status lifecycle beyond a simple pending badge
- No audit trail
- No file upload or document metadata
- No backend service layer
- No advanced validation or compliance controls

## Portfolio Positioning

This project is best positioned as an early prototype that shows initiative, insurance-domain interest, and practical experience connecting a React frontend to a cloud-hosted NoSQL database.

It should be presented as a lightweight precursor to the newer Insurance Claims Management Portal, not as a competing flagship project.
