---

## 🎓 Academic & Group Projects

### 🚀 ESE-SEL-B_Group1 / FlightDiary
Developed as a core group project during my software engineering coursework at the University of Bamberg. **FlightDiary** is a Java-based desktop application designed to record, manage, and analyze flight information with persistent storage, advanced filtering, ranking, and data visualization features. I actively contributed to the team environment, focusing on Git workflow management, data integrity validation, and build configuration.

* 👥 **Team Collaboration:** Developed within a 5-member team (Yuting Song, Yao Guo, Jiyeon Kim, Ellen Maksimovic, Emirhan Karadeniz) using Agile methodologies, incorporating peer code reviews and feature branching.
* 🛠️ **Technical Stack & Specifications:**
  * **Language & GUI:** Java 17 (OpenJDK) with **JavaFX** Framework.
  * **Database:** **SQLite** (Local persistent database initialized automatically at runtime).
  * **Build Tool:** **Gradle** (with Gradle Wrapper) for reproducible builds and automated dependency management.
  * **Code Quality & Linter:** **Spotless** integration for enforcing automatic formatting rules.
  * **Development Environment:** Optimized for import and build management within **IntelliJ IDEA**.
    
* 💻 **Core Engineering & Functionality:**
  * **Data Validation Architecture:** Implemented robust line-by-line validation for external aviation datasets (`.dat` formats for airlines, airports, routes, and planes) to reject corrupted rows while continuing to process valid data.
  * **Concurrency & UI Performance:** Heavy file parsing and data ingestion processes are executed asynchronously outside the JavaFX Application Thread to prevent UI freezing.
  * **Role-Based Access Control:** Separated administrative features (global dataset ingestion) from regular user workflows (maintaining personal diaries, searching, and viewing analytics) to protect overall data integrity.

* 📖 **Application Workflows (User Manual Summary):**
  * **Local-First Architecture:** Operates fully offline; an empty local SQLite database (`flightlog.db`) is automatically initialized on the first launch without external DB setup.
  * **Administrator Workflow:** Admins utilize a dedicated dashboard to ingest global aviation datasets (`airports.dat`, `airlines.dat`, `routes.dat`, `planes.dat`). Malformed rows are skipped automatically with clear warning feedback.
  * **Flight Enthusiast Workflow:** Regular users can browse global routes, search via IATA codes, and log flights into a persistent personal diary.
  * **Map & Advanced Analytics:** Features a dynamic Map View that renders curved flight paths and calculates real-time distances between airports. Includes custom charts (Pie/Bar) for travel patterns and an automated "Top N" filter to rank global airport connectivity based on flight frequencies.

🔒 **Project Status:** The repository is hosted as a Private project on GitLab due to university academic integrity and copyright policies.

🔗 **Repository Link:** [View Project on GitLab](https://gitlab.studium.uni-bamberg.de/ese-sel-b_group1/group1)
