# platform-additional-requirements.md

## 1. Hero / Marketing Copy

### **Hero**
Interactive JS Interview Platform — 30+ coding challenges, instant feedback, AI interview simulation, competitive leaderboards, and automated testing. From beginner to advanced with real-world scenarios.

### **Sub-Hero**
Practice real interview problems inside a browser editor, get instant test results, simulate live interviews with AI, and climb public/company leaderboards. Build skills, confidence, and a portfolio recruiters notice.

### **Primary CTAs**
- **Start Free Challenges**
- **Try AI Interview**

---

## 2. Information Architecture (Pages & Key UI)

### **Home / Landing Page**
- Hero section
- Features overview
- Top challenges
- Testimonials
- Call-to-actions

### **Challenges Page**
- Filters: difficulty, tags, package, popularity
- Challenge list
- Progress indicators and badges

### **Challenge Detail Page**
- Problem statement
- Learning materials
- Test cases
- Code editor
- Run & Submit buttons

### **AI Interview Simulator**
- Choose difficulty, duration, interview style
- Live Q&A interface
- Feedback report

### **Debug Practice**
- Broken code challenge
- Patch and fix system

### **Leaderboard Page**
- Global leaderboard
- Friends leaderboard
- Company-private leaderboard

### **Learning Paths**
- Fundamentals
- Async & Promises
- Frontend Patterns
- Node.js APIs

### **Account Page**
- Profile
- Progress tracking
- Badges
- Settings

### **Docs / Pricing / How It Works**

---

## 3. Feature Design & UX Flows

### **A. Challenge Flow (Instant Feedback)**
1. User opens a challenge.
2. Sees problem, constraints, examples & tips.
3. Runs sample tests with **Run** (visible tests only).
4. Submits with **Submit** for full hidden + visible test suite.
5. Results include:
   - Pass/fail per test
   - Expected vs actual
   - Runtime & memory
   - Score
6. Optional hints after attempts/time penalties.

### **B. AI Interview Simulator**
- User selects: difficulty, time, style (algo / system / debugging).
- AI interviewer asks questions and follow-ups.
- Session timed, with transcript.
- Final report includes:
  - Score breakdown
  - Code quality notes
  - Time management
  - Suggested improvements
- Option to save/record the session.

### **C. Competitive Leaderboards**
- Global rankings
- Weekly mini-contests
- Private company leaderboards
- Achievements & badges

### **D. Automated Testing & Security**
- Multi-layer tests: sample, full, hidden edge
- Sandboxed JS runner (Node VM, containers, or workers)
- No network or filesystem access
- Performance & memory limits

---

## 4. Challenge Catalogue (30+ Challenges)

### **Beginner (10 Challenges)**
1. Sum of Two Numbers
2. Reverse a String
3. Binary Search
4. Palindrome Checker
5. Word Frequency Counter
6. Greedy Coin Change
7. Temperature Converter
8. Array Flatten (1-level)
9. Employee Data CRUD
10. Find Duplicates

### **Intermediate (12 Challenges)**
11. Two-Sum with Indices
12. String Pattern Matching
13. Polymorphic Shape Calculator
14. Slice/Splice Tasks
15. Circuit Breaker Pattern
16. Performance Loop Optimization
17. Promise Pool
18. Debounce & Throttle
19. SQL-like Query on Array Objects
20. LRU Cache
21. Microservice API Mock (Express)
22. Go-Style Context Cancellation

### **Advanced (10+ Challenges)**
23. OAuth2 Mock Auth System
24. Dynamic Programming: LIS
25. Graph Shortest Path
26. Token Bucket Rate Limiter
27. Cache with Multiple Eviction Policies
28. WebSocket Chat Server
29. File Processing Pipeline
30. Regex Text Processor
31. Concurrent Task Orchestrator
32. Memory-Safe Streaming Parser

Each challenge includes:
- Description
- Constraints
- Sample inputs/outputs
- Learning materials
- Visible tests
- Hidden tests
- Hints

---

## 5. Scoring, Tests & Hidden Test Strategy

### **Scoring Model**
- **Correctness**: primary score weight
- **Performance**: time + space bonuses
- **Code quality**: linting suggestions
- **Attempts/time**: fewer attempts = small bonus

### **Test Strategy**
- **Sample tests**: visible (Run)
- **Full tests**: visible + hidden (Submit)
- **Hidden edge tests**: large inputs, fuzz tests, stress cases

### **Automated Grading System**
- Runs tests in isolated sandbox
- Each test returns:
  - pass/fail
  - output diff
  - runtime & memory

### **Cheating Prevention**
- Solution hashing
- Similarity detection
- Randomizing hidden test parameters each run

---

## 6. Tech Stack & Infrastructure

### **Frontend**
- React + TypeScript
- Vite
- Tailwind CSS
- Monaco Editor
- WebSocket for realtime updates

### **Backend**
- Node.js + TypeScript
- Express or NestJS
- Containerized sandbox runners
- Custom test harness
- AI integration with OpenAI or similar

### **Data & Infra**
- PostgreSQL
- Redis (queues, caching)
- S3 storage
- CI/CD with GitHub Actions
- Monitoring: Sentry, Prometheus, Grafana

### **Security**
- Strong sandbox isolation
- No external network access
- CPU & memory limits
- Rate limiting

### **Optional Enhancements**
- Automated code review engine
- Keyboard shortcuts for coding contests

---

## 7. Example UI Copy for Challenge Detail

### **Title**: Promise Pool — Limit Concurrent Promises
### **Difficulty**: Intermediate

**Description:**
Implement a function `promisePool(tasks, n)` that runs at most **n** promise-returning tasks at the same time and resolves when all tasks complete. It should return the results in the same order as the input.

**Sample I/O:**
```
Input:
  tasks = [() => Promise.resolve(1), ...], n = 2
Output:
  Promise that resolves to [1, ...]
```

**Learning Materials:**
- Concurrency patterns in JS
- Promise.allSettled
- Async/await best practices

---

## 8. Monetization & Product Options

### **Free Tier**
- Beginner challenges
- 3 AI interview simulations per month

### **Pro Tier**
- All challenges unlocked
- Unlimited AI interviews
- Private leaderboards
- Company workspace features

### **Team / Enterprise**
- Private space
- Custom challenge sets
- SSO
- Exportable leaderboards

---

## 9. Next Steps (Choose One)
- **A. Generate 30+ challenge JSON** (import-ready)
- **B. Full React landing page + challenge list UI**
- **C. AI Interview prompt templates + scoring logic**
- **D. Full technical spec (API + DB Schema + workers)**

Tell me which you want next!
