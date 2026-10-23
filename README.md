# Leave Management System

A leave request and approval system built using **Camunda 8, Spring Boot, and React**. The application allows employees to submit and track leave requests, while managers can review and approve or reject applications.

## Tech Stack
- Camunda 8 (Docker) – Workflow engine
- Spring Boot – Backend
- React with Vite – Frontend
- PostgreSQL – Database

## Features
- Leave application and request tracking
- Manager approval and rejection
- Leave balance management
- BPMN-based approval workflow

## How to Run

### 1. Start Camunda
```bash
cd camunda && docker compose up -d
```

### 2. Start Backend
```bash
cd backend && mvn spring-boot:run
```

### 3. Start Frontend
```bash
cd frontend && npm install && npm run dev
```

## Application Links
- **Frontend:** http://localhost:5173
- **Backend:** http://localhost:8081
- **Camunda Operate:** http://localhost:8080/operate

## Workflow
Leave Request → Validate Leave → Manager Approval → Finalize Request

**BPMN Process ID:** `leave-request`

**BPMN File:** `bpmn/leave-request.bpmn`
