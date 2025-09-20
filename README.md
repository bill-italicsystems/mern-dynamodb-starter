// ======================================
// Full Stack MERN (React + Node + DynamoDB) Coding Assignment
// ======================================

/*
🧪 PURPOSE:
To assess how the candidate:
- structures a small full-stack project
- uses modern React and Node.js effectively
- integrates with AWS DynamoDB (via SDK)
- approaches problem solving, async handling, and error management
- writes clean, readable, and testable code

Candidates may use docs, StackOverflow, and any reference materials.
*/

// ======================================
// 📄 ASSIGNMENT OVERVIEW
// ======================================
/*
Build a simple Task Manager application with the following features:

1. Frontend (React):
  - Display all tasks (title, status)
  - Form to add new task (title, optional description)
  - Mark task as complete/incomplete
  - Delete task

2. Backend (Node.js):
  - Expose REST endpoints:
    - GET /tasks
    - POST /tasks
    - PUT /tasks/:id
    - DELETE /tasks/:id
  - Connect to DynamoDB using AWS SDK

3. Database (DynamoDB):
  - Table: tasks
    - id (string, UUID)
    - title (string)
    - description (string, optional)
    - status (string: 'pending' | 'done')
    - createdAt (ISO string)

Optional (Bonus):
- Add pagination support
- Add userId for multi-user support
- Add environment-based config (dev/prod)
*/

// ======================================
// 📂 FILE STRUCTURE (Suggested)
// ======================================
/*
project-root/
├── client/ (React)
│   ├── src/
│   │   ├── components/
│   │   ├── pages/
│   │   ├── api/ (optional)
│   │   ├── App.js
│   │   └── index.js
├── server/ (Node.js)
│   ├── index.js
│   ├── routes/
│   ├── controllers/
│   ├── db/
│   │   └── dynamodb.js
│   └── utils/
├── .env.template
├── README.md
└── package.json
*/

// ======================================
// 🔧 TECHNICAL EXPECTATIONS
// ======================================
/*
Frontend:
- React functional components
- useState, useEffect, and fetch or axios
- Minimal styling required (Tailwind/Bootstrap/plain OK)

Backend:
- Node.js + Express
- REST API with proper status codes
- Error handling
- DynamoDB integration via AWS SDK v3 (preferred)
- Use UUID for task ID generation

Other:
- Use .env for secrets (AWS keys if mocked/real used)
- Provide sample test data or seeding logic if time permits
- GitHub repo with meaningful commits is ideal
*/

// ======================================
// 📝 SUBMISSION INSTRUCTIONS
// ======================================
/*
- Fork or clone the provided repo
- Complete the assignment within the given time (2–3 hours)
- Push your code to a private repo (GitHub/GitLab)
- Share the repo link + README with instructions to run locally
- Optionally record a 5–10 min video explaining your approach
*/

// ======================================
// ▶️ FULL SETUP & RUN INSTRUCTIONS
// ======================================
/*
1. Install dependencies:
   cd client && npm install
   cd ../server && npm install

2. Setup environment variables:
   - Create a `.env` file in the root directory
   - Copy content from `.env.template`
   - Add your AWS credentials (or leave blank if mocking)

3. Start backend:
   cd server && npm start

4. Start frontend:
   cd client && npm start

5. Open http://localhost:3000 in your browser to access the app.

6. If using mock DynamoDB (optional):
   - Install Docker and run `dynamodb-local` container
   - Point your SDK config to the local endpoint
*/

// ======================================
// 🧑‍⚖️ GRADING RUBRIC (Internal)
// ======================================
/*
1. Project structure & modularity – 20%
2. Working REST API with basic CRUD – 25%
3. Frontend interaction with API – 20%
4. DynamoDB integration – 15%
5. Code readability & error handling – 10%
6. Optional bonus features – 10%
*/
