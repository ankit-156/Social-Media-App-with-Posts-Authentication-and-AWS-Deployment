SocialConnect demo (frontend + backend)
=====================================

What you get:
- client/: Vite + React frontend (simple UI, no build tooling beyond Vite)
- server/: Express backend with JWT auth and in-memory store
- A single zip you can download and run locally for development

Quick start (local)
-------------------
1. Start backend:
   cd server
   npm install
   npm run start

2. Start frontend:
   cd client
   npm install
   npm run dev

By default the frontend expects the API at http://localhost:5000
You can change this by setting REACT_APP_API environment variable before running Vite.

Notes:
- This project uses an in-memory store for users and posts (for demo). To persist data, replace the server store with MongoDB or another DB.
- For production, change JWT_SECRET, enable HTTPS, use a real DB, and secure file uploads.
- To deploy on AWS: you can host the server on an EC2/Elastic Beanstalk or containerize it for ECS, and host the frontend on S3 + CloudFront or deploy as a static site.

