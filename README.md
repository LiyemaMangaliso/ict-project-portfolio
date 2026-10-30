# ict-project-portfolio
## 2. User Stories and Tasks

### Evidence

Based on our community questionnaire data gathered from Khayelitsha residents, we identified two critical user requirements. Below are the resulting Agile User Stories broken down into engineering and design tasks:

#### User Story 1: Fast Reporting of Burst Drainpipes
*   **As a** Khayelitsha resident affected by street flooding,
*   **I want** to quickly report a burst or overflowing drainpipe via a mobile platform with location pinning,
*   **So that** municipal response teams are notified instantly to fix it faster.

**Actionable Tasks:**
- [ ] **Task 1 (UI/UX):** Design a lightweight, mobile-responsive reporting form featuring fields for severity level and photo uploads.
- [ ] **Task 2 (Frontend):** Integrate a geolocation/GPS tagging feature to automatically capture the exact coordinates of the burst pipe.
- [ ] **Task 3 (Backend):** Develop a database schema and API endpoint to store report inputs (location, timestamp, description, and status).

#### User Story 2: Tracking Repair Progress
*   **As a** community member navigating local streets,
*   **I want** to track the live progress and status of a reported pipe repair,
*   **So that** I know when the hazard will be cleared and the street will be safe again.

**Actionable Tasks:**
- [ ] **Task 1 (Database):** Configure dynamic status categories in the backend pipeline (`Reported`, `Dispatched`, `In Progress`, `Resolved`).
- [ ] **Task 2 (Notification Engine):** Implement a automated SMS or push notification service to alert the reporter when status updates occur.
- [ ] **Task 3 (UI/Dashboard):** Build a public dashboard or map visualization interface showing active and resolved maintenance tickets in the area.

---

### Reflection

The questionnaire acted as our primary data source to justify the creation of these specific user stories. By reviewing respondent feedback—specifically regarding how slow pipe repairs take and the severe disruptions caused by overflowing streets—we were able to extract real community pain points and frame them into user-centric requirements using the standard Agile framework.

Breaking these user stories down into discrete, manageable tasks allowed our development team to bridge the gap between user needs and technical implementation. It ensured that every UI design decision and backend feature directly answered a complaint raised in our Khayelitsha community survey. This process highlighted how vital user empathy and clear task division are in Agile project management to prevent feature creep and keep development goals aligned.

## 3. Product Backlog

### Evidence

The following is our prioritised Product Backlog for the Khayelitsha Drainage Reporting and Repair Tracking System. The items are ordered by priority (High, Medium, Low) based on core system requirements and critical user needs identified from our survey.

| ID | Item Name / Feature | Description | Priority | Target Sprint |
| :--- | :--- | :--- | :--- | :--- |
| **PBI-01** | User Report Submission Form | A mobile-friendly form allowing users to select incident severity and write descriptions of burst drainpipes. | **High** | Sprint 1 |
| **PBI-02** | GPS & Geolocation Tagging | Integration of location pinning API to capture exact coordinates of the overflowing drainpipes. | **High** | Sprint 1 |
| **PBI-03** | Database Setup & Reporting API | Core backend database architecture to securely capture, store, and manage user reports and media uploads. | **High** | Sprint 1 |
| **PBI-04** | Municipal Admin Dashboard | A secure web portal for municipal maintenance teams to view incoming reports, assign field technicians, and change task statuses. | **Medium** | Sprint 2 |
| **PBI-05** | Real-time Status Tracker | A public page or tracking timeline where residents can view the live progress (`Reported` to `Resolved`) of their specific ticket. | **Medium** | Sprint 2 |
| **PBI-06** | SMS Notification Engine | An automated text service that messages the reporter whenever the status of their reported drainage pipe updates. | **Medium** | Sprint 3 |
| **PBI-07** | Public Interactive Incident Map | A visual map layer (e.g., Leaflet or Google Maps API) displaying active and resolved drainage leaks across Khayelitsha. | **Low** | Sprint 3 |
| **PBI-08** | Municipal Analytical Reporting | A tool for generating monthly reports showing breakdown hotspots, average response times, and resolution rates. | **Low** | Sprint 4 |

---

### Reflection

The Product Backlog served as the definitive "single source of truth" for our system's entire scope. Creating this backlog required our team to look beyond immediate features and map out everything needed to build a fully functional product. By structuring the backlog as an ordered list, we were forced to make strategic decisions regarding value versus effort. High-priority items were reserved for core functionality—such as the submission form and geolocation pinning—without which the platform could not solve the community's primary pain point.

Managing this backlog gave us valuable insight into how Agile accommodates project evolution. As we moved items down into lower-priority tiers (like analytical reporting and automated text notifications), we learned how to effectively manage project constraints and avoid feature creep. This process ensured that the development team focused on delivering a viable product that addresses slow municipal response times before working on supplementary, nice-to-have features.


```markdown
## 4. Sprint Backlog

### Evidence

The following table represents our Sprint 1 Backlog for the Khayelitsha Drainage System. It shows the specific technical and operational tasks selected from our high-priority backlog, alongside their assigned team member, estimated effort (in Story Points), and real-time development status.

| Task ID | Related PBI | Task Description | Assigned To | Effort (SP) | Status |
| :--- | :--- | :--- | :--- | :--- | :--- |
| **TSK-101** | PBI-01 | Design wireframes and user flow for the mobile submission form. | UI/UX Designer | 3 | **Done** |
| **TSK-102** | PBI-01 | Implement frontend HTML/CSS/JS form fields for severity and descriptions. | Frontend Dev | 5 | **In Progress** |
| **TSK-103** | PBI-02 | Research and integrate geolocation browser API for capturing coordinates. | Frontend Dev | 5 | **In Progress** |
| **TSK-104** | PBI-03 | Design relational database schema for storing incident report tables. | Backend Dev | 3 | **Done** |
| **TSK-105** | PBI-03 | Set up express server, POST api route, and connect database pipelines. | Backend Dev | 8 | **To Do** |
| **TSK-106** | PBI-02 | Write server validation logic to handle incoming coordinates payload safely. | Backend Dev | 2 | **To Do** |
| **TSK-107** | PBI-04 | Engage municipality stakeholders to secure a collaboration framework and transition plan for the sewage pipe repair reporting website. | Product Owner / PM | 5 | **In Progress** |

---

### Reflection

The Sprint Backlog acted as our operational, day-to-day action plan during our active development phase. While the Product Backlog focused on the broader vision of the Khayelitsha drainage solution, the Sprint Backlog forced us to focus entirely on near-term execution. Breaking high-level features down into atomic developer tasks allowed us to assign explicit responsibilities and realistic timelines to individual team members, making overall project tracking significantly more transparent.

By utilizing this backlog, we learned that a successful Agile sprint involves both technical engineering tasks and vital operational dependencies. Including stakeholder engagement (TSK-107) directly alongside coding tasks ensured that the development team remained aligned with the City of Cape Town municipality's real-world operational constraints and transition requirements. Categorizing development items into active buckets—`To Do`, `In Progress`, and `Done`—reduced team friction and gave us an instant, highly visual representation of our current project velocity. This structure kept us focused on building a viable, deployable architecture while simultaneously preparing the framework for actual municipal adoption.

