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
