# Ashivam-website
Responsive portfolio for Ashivam Technologies, featuring services, industry solutions, projects, careers, and internships. Built with HTML, Tailwind CSS, and JavaScript. Contact links open prefilled email drafts. Photos load from Unsplash.
Ashivam Technologies — Official Platform
Enterprise Technology & Software Studio Platform. Built with a high-performance React 18 frontend and a hardened Express 5 / MongoDB REST API backend.

CI Status Production Node Express MongoDB Tests

🏛️ Architecture & Platform Overview
The repository consists of two integrated tiers:

Frontend (/src): Single-Page Application (SPA) designed as a luxury dark-mode corporate tech studio interface with fluid responsive layouts (320px to 4K ultrawide), micro-interactions, and real-time contact validation.
Backend (/backend): Production-grade REST API utilizing ES Modules, Mongoose document modeling, JWT authentication, granular RBAC, tiered rate limiting, and structured error handling.
🛠️ Technology Stack
Frontend
Framework: React 18.3.1
Bundler: Vite 5.4.21
Styling: Modular CSS architecture with design tokens (globals.css, animations.css)
Typography: Space Grotesk, Inter, JetBrains Mono
API Client: Native fetch with AbortController timeout & standardized error mapping (src/api.js)
Backend
Framework: Express 5.2.1 (Node.js ES Modules)
Database: MongoDB via Mongoose 9.10.3
Security: Helmet, Multi-Origin CORS whitelist, express-rate-limit, input sanitization, ReDoS mitigation
Authentication: HMAC SHA-256 JWT, bcryptjs password hashing (cost factor 12)
File Uploads: Multer with strict MIME and extension validation (.pdf, .doc, .docx)
Testing: Node.js native test runner (node:test), Supertest, node:assert/strict
Observability: Correlation ID tracing (X-Request-Id) across all endpoints and logs
🚀 Quick Start & Development
1. Frontend Setup
# Install dependencies
npm install

# Run Vite development server (http://localhost:5173)
npm run dev

# Build for production
npm run build
2. Backend Setup
# Navigate to backend
cd backend

# Install dependencies (0 vulnerabilities verified)
npm install

# Setup environment configuration
cp .env.example .env

# Run automated tests
npm test

# Seed initial Superadmin account (requires running MongoDB instance)
npm run seed

# Start development server with hot-reload (http://localhost:5000)
npm run dev
🧪 Testing Commands
The backend includes a comprehensive, automated test suite:

cd backend

# Run all 24 unit, integration, and security tests
npm test

# Run validation & query unit tests
npm run test:unit

# Run API endpoints integration tests
npm run test:integration

# Run security headers & rate limiting tests
npm run test:security
Test Status: 24/24 Passing (0 failures, 1.8s execution)

📚 Engineering Documentation
Comprehensive specifications and audit logs are available in docs/:

Document	Description
BACKEND-AUDIT.md	Initial architectural audit and vulnerability remediation plan
API.md	Complete REST API specification, schemas, headers, status codes
DATABASE-DESIGN.md	Database models, Mermaid ER diagrams, indexes, and compound keys
API-SECURITY-AUDIT.md	OWASP API Security Top 10 analysis and threat mitigation matrix
ENVIRONMENT.md	Environment variables matrix, security practices, and production guide
BACKEND-TEST-REPORT.md	Automated test execution transcript and contract validation
🌐 Deployments
Live Production: https://ashivam-tec-h.vercel.app
Continuous Integration: Automated GitHub Actions pipeline verifying frontend builds, backend tests, and vulnerability scans on every push to main.
About
ashivam-tec-h.vercel.app
Resources
Readme
Activity
Stars
0 stars
Watchers
0 watching
Forks
0 forks
Report repository
Releases
No releases published
Deployments
30
 (30)
Production
5 hours ago
Packages
No packages published
Contributors
1
 (1)
@Ritikgupta-tech
Ritikgupta-techRitik Gupta
Languages
JavaScript
61.5%
HTML
27.5%
CSS
10.9%
Dockerfile
0.1%
Footer
© 2026 GitHub, Inc.
