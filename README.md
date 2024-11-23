# obwob: Feature Showcase

Welcome to the **obwob** showcase repository. This repository demonstrates key features and technical architecture of obwob, a proprietary application designed for event coordination and participant engagement, intended for future commercialization. 

## Purpose
The purpose of this repository is to demonstrate the capabilities of the application to potential employers, collaborators, and recruiters. It includes examples and partial implementations of functionality but does not contain the full codebase or deployment-ready materials for the application.

## About obwob
**obwob** is a platform that facilitates:
- Event creation and management by coordinators.
- Participant registration and engagement via a mobile progressive web app (PWA).
- Real-time question delivery and response collection during events.

The system is built using:
- **Backend**: Django and Ruby on Rails.
- **Frontend**: React.
- **Database**: MariaDB.

This repository includes selected components and examples to highlight functionality while preserving the integrity of the proprietary codebase.

## Repository Highlights
Example implementations of participant registration, event creation, and live question pushing.
Demonstrations of the UI/UX principles and technical skills applied in the full application.
Clear documentation of design decisions and implementation strategies.

## Disclaimer
This repository does not include the complete obwob codebase. It is intended solely to showcase features and capabilities to potential employers, collaborators, and recruiters.

## License
All rights reserved. The contents of this repository are for demonstration purposes only and may not be copied, distributed, or used for commercial or non-commercial purposes without explicit permission from the owner.

## Contact
For more information or inquiries, please contact Laura Gates on [LinkedIn: linkedin.com/in/laurapg1214](https://linkedin.com/in/laurapg1214).

---

## Features Overview

**obwob** simplifies event coordination and participant engagement with the following features:  

1. **Event Management**
   - Create, edit, and organize events under a specific organization.
   - Manage participants, facilitators, and coordinators.  

2. **QR Code Integration**
   - Seamless participant and facilitator login using QR codes.  

3. **Live Interaction**
   - Facilitators can push questions to participant devices in real-time.
   - Participants respond directly via a Progressive Web App (PWA).  

4. **Cross-Platform Compatibility**
   - **Django** backend powers a React Single Page Application (SPA).
   - **Ruby on Rails PWA** handles participant and facilitator interactions.

5. **Dynamic Reporting**
   - Coordinators access detailed reports of participant responses and event statistics.  

---

## Technical Highlights

This section highlights the app's architecture and tech stack:

- **Backend**:
  - [Django REST Framework](https://www.django-rest-framework.org/) with a service-oriented architecture.
  - Custom authentication and role management for admin, coordinators, facilitators, and participants.
- **Frontend**:
  - React SPA (for coordinators) built with reusable, feature-based components.
  - Ruby on Rails PWA (for participants/facilitators) optimized for offline use.
- **Database**:
  - Centralized data storage with MariaDB for seamless synchronization.
- **DevOps**:
  - CI/CD pipelines with GitHub Actions.
  - Deployed on [platform] (e.g., AWS/Heroku/Vercel).

---

## Repository Content

This repository includes:  

1. **Sample Code**
   - Snippets demonstrating key components (e.g., QR code scanner, live question-pushing system).  
   - Example Django model for events:
     ```python
     class Event(models.Model):
         id = models.UUIDField(primary_key=True, default=uuid.uuid4, editable=False)
         name = models.CharField(max_length=200)
         organization = models.ForeignKey(Organization, on_delete=models.CASCADE)
         created_at = models.DateTimeField(auto_now_add=True)
     ```
     
2. **Screenshots and Diagrams**
   - `/screenshots`: Interface previews (React SPA, Rails PWA).
   - `/diagrams`: Architecture and database relationship diagrams.

3. **Documentation**
   - [API Workflow](./docs/api-workflow.md): How the React SPA and Rails PWA interact with the Django backend.
   - [Sample UI Flows](./docs/ui-flows.md): Screenshots and descriptions of key user workflows.

---

## Screenshots

### React SPA (Coordinator View)
![Coordinator Dashboard](./screenshots/coordinator-dashboard.png)

### Rails PWA (Participant View)
![Participant Response](./screenshots/participant-response.png)

---

## Try it Out!

- **Demo Version**: [Live Demo](https://demo-link.example.com)
- **GitHub Pages**: [Feature Overview](https://laurapg1214.github.io/obwob-showcase)

---

## Development Setup

Follow these steps to set up a local environment for the demo app:  

1. Clone the repository:
   ```bash
   git clone https://github.com/laurapg1214/obwob-showcase.git
   cd obwob-showcase
   ```
2. Install dependencies:
   ```bash
   npm install  # For React components
   ```
3. Run the app locally:
   ```bash
   npm start
   ```

---

## Contact

If you have questions or would like to learn more about **obwob**, feel free to connect with me on [Linked in: linkedin.com/in/laurapg1214](https://linkedin.com/in/laurapg1214).

