# Group 42: Contribution Guidelines & Workflow

Welcome to the **Air Quality & Pollution Health Advisor** repository! 

Because we have an eight-person development team collaborating on this project, we must follow a strict Git workflow. This ensures that no one accidentally overwrites another person's code, prevents frustrating merge conflicts, and keeps our main application stable at all times.

**⚠️ STRICT RULE: The `main` branch is protected.** 
You cannot push code directly to `main`. All changes must be made on a separate feature branch and submitted via a Pull Request (PR) for review by the Project Leader (Abdulmalik).

---

## 🏗️ Module & File Assignments

To prevent code conflicts, **you must only write code inside your assigned file**. Do not modify `app.py` or any files assigned to other team members unless you have explicitly discussed it with the Project Leader.

| Team Member | Project Role | Assigned File(s) |
| :--- | :--- | :--- |
| **Abdulmalik Haruna** | Lead Architect & System Assembly | `app.py`, `ai_helper.py` |
| **Samuel Essien** | Data Acquisition & API Client | `api_client.py` |
| **Aliyu Madugu** | Data Models & OOP | `models.py` |
| **Victor Adejoh** | Domain Logic & Risk Analyzer | `risk_logic.py` |
| **Goodluck Titus** | Input Validation & Utilities | `validation.py` |
| **Miracle Oji** | Persistence & Storage Layer | `storage.py` |
| **Kelechi Obialor** | UI - Main Dashboard | *Coordinate with Lead in `app.py`* |
| **Emmanuel Solomon**| UI - Comparison & History | *Coordinate with Lead in `app.py`* |

---

## 🔄 The Standard Development Workflow

Please follow these exact steps every single time you work on the project.

### 1. Clone the Repository (First Time Only)
Open your terminal/command prompt and clone the repository to your local machine:
`git clone https://github.com/nuraddeen2014/air-quality-adviser.git`
`cd air-quality-adviser`


### 2. ALWAYS Pull the Latest Code (Before You Start Coding)
Before you write a single line of code for the day, ensure you have the newest updates from the rest of the team.
`git checkout main`
`git pull origin main`


### 3. Create Your Working Branch
Never work directly on the `main` branch. Create a new branch named after your name and the feature you are currently building.
`git checkout -b [your-name]-[feature-name]`
*(Example: `git checkout -b samuel-api-fetch`)*
*(Example: `git checkout -b miracle-json-save`)*


### 4. Write Your Code
Work only inside your assigned `.py` file. Run your code locally to ensure it works correctly and doesn't crash before moving to the next step. 

### 5. Commit and Push Your Work
Once your code is ready and tested, stage, commit, and push it to your specific branch on GitHub.
`git add .`
`git commit -m "Briefly describe what you coded (e.g., Added fetch function for API)"`
`git push origin [your-name]-[feature-name]`


### 6. Open a Pull Request (PR)
1. Go to the repository page: https://github.com/nuraddeen2014/air-quality-adviser
2. You will see a green **Compare & pull request** button appear near the top. Click it.
3. Give your PR a clear title.
4. Leave a brief comment explaining what you built.
5. Click **Create pull request**.

### 7. Review and Merge
The Project Leader will review your Pull Request. 
* If the code is good and doesn't conflict, it will be merged into `main`. 
* If changes are needed, you will receive feedback in the PR comments. To fix it, simply make the changes on your computer, save, commit, and push again. The PR will update automatically.

---

**🛑 Crucial Rule:** If you are ever unsure about a Git command, run into an error, or don't know where your code should go, **stop and ask in the Group 42 chat** before pushing. Let's build something great!