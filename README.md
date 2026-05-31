# API Testing with Postman & Newman
Automated API testing using Postman collections and Newman CLI.

## Overview
This project validates JSONPlaceholder REST endpoints with 6 test cases covering CRUD and query operations.

## Tech Stack
- Postman Collection v2.1
- Newman CLI
- Node.js 14+

## Setup
```bash
npm install
npm test
```

## Scripts
- `npm test` → CLI + HTML report (`results/report.html`)
- `npm run test:html` → HTML only
- `npm run test:json` → JSON only
- `npm run test:all` → HTML then JSON

## Test Cases
- TC-API-001: GET `/posts`
- TC-API-002: GET `/posts/{id}`
- TC-API-003: POST `/posts`
- TC-API-004: PUT `/posts/{id}`
- TC-API-005: DELETE `/posts/{id}`
- TC-API-006: GET `/posts?userId=1&_limit=5`

## Reports
- HTML: `results/report.html`
- JSON: `results/report.json`

## Project Structure
```text
api-testing-postman/
├── postman/
│   ├── collection.json
│   └── environment.json
├── results/
├── tests/
│   └── test-data.json
├── documentation/
│   ├── API_ENDPOINTS.md
│   └── TEST_CASES.md
├── package.json
├── .env.example
└── README.md
```
