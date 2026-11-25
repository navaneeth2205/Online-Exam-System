<div align="center">

<img src="https://capsule-render.vercel.app/api?type=waving&color=gradient&customColorList=4,12,24,30&height=220&section=header&text=Online%20Examination%20System&fontSize=42&fontColor=ffffff&animation=twinkling" width="100%" alt="Online Examination System" />

# 🎓 Online Examination System

<p align="center">
  <a href="https://github.com/navaneeth2205/Online-Exam-System/releases/latest">
    <img src="https://img.shields.io/badge/Release-v1.1.0-3b82f6?style=for-the-badge&logo=github&logoColor=white" alt="Latest Release" />
  </a>
  <a href="https://github.com/navaneeth2205/Online-Exam-System/releases/download/v1.1.0/OnlineExamSystem-v1.1.0-Windows.zip">
    <img src="https://img.shields.io/badge/Download-Standalone%20App%20(ZIP)-10b981?style=for-the-badge&logo=windows&logoColor=white" alt="Download Windows Release" />
  </a>
  <img src="https://img.shields.io/badge/Java-17%2B-f97316?style=for-the-badge&logo=openjdk&logoColor=white" alt="Java 17+" />
  <img src="https://img.shields.io/badge/Database-MySQL%208.0-0284c7?style=for-the-badge&logo=mysql&logoColor=white" alt="MySQL 8.0" />
  <img src="https://img.shields.io/badge/License-MIT-8b5cf6?style=for-the-badge" alt="License" />
</p>

</div>

---

## 🚀 Core Innovations

<table width="100%">
<tr>
<td width="50%" valign="top">

### 🛡️ Multi-Channel Proctoring Engine
- **JVM Window Focus Interceptor**: Real-time detection of OS window deactivations (`Alt + Tab`, Windows key, application switching) via `WindowFocusListener`.
- **Global Keystroke Filtering**: Hooks `KeyboardFocusManager` to block cheating shortcuts (`Ctrl + C`, `Ctrl + V`, `Alt + F4`, function keys).
- **Automated Webcam Surveillance**: Background daemon capturing periodic visual surveillance frames with dynamic threat index scoring.
- **3-Strike Kiosk Termination**: Automatically terminates testing session and executes atomic submission upon exceeding candidate violation thresholds.

</td>
<td width="50%" valign="top">

### 🔐 Cryptographic Defense & Session Integrity
- **PBKDF2-HMAC-SHA256**: 120,000 iterative key-stretching rounds via `javax.crypto.SecretKeyFactory` to defeat GPU/ASIC brute-force cracking.
- **128-Bit CSPRNG Salts**: Cryptographically secure salts generated per account via `java.security.SecureRandom`.
- **Transparent Migration**: Automatically upgrades legacy credentials to PBKDF2 upon successful candidate authentication.
- **Concurrent Session Locking**: Validates active UUID tokens and runs 30-second heartbeat pings to eliminate multi-device proxy logins.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### 📊 Psychometric Item Analytics (CTT)
- **Facility Value (Item Difficulty)**:
  $$\mathbf{P = \frac{R}{N}}$$
  *Algorithms automatically classify items into Optimal, Easy, or Ambiguous difficulty tiers.*
- **Discrimination Index ($\mathbf{D}$)**:
  $$\mathbf{D = \frac{U - L}{N_G}}$$
  *Calculates item discrimination power between upper and lower 27% student cohorts (Kelley's Rule).*
- **Distractor Efficiency Audit**: Identifies dead choices and highlights confusing answer alternatives.

</td>
<td width="50%" valign="top">

### 📜 Tamper-Proof Vector Certification
- **Dynamic PDF Compilation**: Automated vector PDF credential rendering with candidate metrics, grade badges, and institutional seals.
- **SHA-256 Digital Fingerprint**: Computes unique cryptographic integrity checksum across student ID, exam ID, and score.
- **2D QR Matrix Verification**: High-density QR matrix verifiable against official database records via `VerifyCertificateUI.java`.
- **Public & Admin Ledger**: Real-time authenticity lookup eliminating fraudulent academic credentials.

</td>
</tr>
<tr>
<td width="50%" valign="top">

### ⚡ Zero-Latency Desktop Experience
- **FlatLaf Modern Design System**: Clean light SaaS theme, sub-pixel LCD font anti-aliasing hints, and responsive glassmorphic cards.
- **EDT Concurrency Isolation**: Cryptographic PBKDF2 hashing (120,000 iterations), candidate registration, and multi-query metrics are fully offloaded to asynchronous `SwingWorker` background threads, keeping the Event Dispatch Thread completely free and maintaining 60 FPS responsiveness.
- **Hardware-Cached I/O & Pre-Warming**: DirectShow webcam driver scanning is cached and pre-warmed in the background, eliminating hardware device discovery stalls.
- **Optimized Particle Engine**: `AuroraBackground.java` renders at 24 FPS with automatic render throttling when minimized, cutting background CPU utilization by ~30%.
- **Custom Java2D Polar Graphics**: Trigonometric multi-axis competency radar projection visualizing candidate skill distribution.

</td>
<td width="50%" valign="top">

### 🔄 Resilient Persistence & Transactions
- **High-Performance Connection Pool**: Centralized thread-safe connection pool in `DBConnection.java` with dynamic proxy connection reuse and asynchronous socket pre-warming, cutting database query latency to ~5 ms without TLS handshake overhead.
- **Automated Server Lifecycle**: One-click launchers (`run.ps1` & `run.bat`) automatically detect port 3306 and spin up the local MySQL 8.0 daemon if it is not already running.
- **Two-Phase Atomic Transactions**: Full `COMMIT` and `ROLLBACK` guarantees saving exam attempts and individual responses synchronously.
- **Idempotent Schema Migration**: `SchemaMigrator.java` dynamically evolves table structures and seeds catalogs at startup with zero data loss.

</td>
</tr>
</table>

---

## 📂 Project Directory Structure

```
Online-Exam-System/
├── java files/                           # All 49 Java source files organized into canonical packages
│   ├── com/onlineexam/
│   │   ├── main/                         # Bootstrap & Application Lifecycle (Main.java)
│   │   ├── dao/                          # Database Access, PBKDF2 Hashing, Sessions, & CTT (12 classes)
│   │   ├── data/                         # Domain Models, In-Memory State & PDF Builder (4 classes)
│   │   └── ui/                           # Design Tokens, Glassmorphism & Animations (13 classes)
│   │       ├── student/                  # Candidate Dashboard, Proctored Runner & Scorecards (9 classes)
│   │       └── admin/                    # Admin Command Center, Proctor Logs & Analytics (8 classes)
│   └── TestDB.java                       # Database Diagnostic Utility (1 class)
│
├── sql/                                  # Relational Database Migration & Seed Scripts
│   ├── database_setup.sql                # 8 Normalized InnoDB Tables & Foreign Keys
│   └── sample_data.sql                   # Default Admin/Student Accounts & 100 Sample MCQs
│
├── docs/                                 # Project Report & Academic Publication (PDF)
│   └── Online Examination Management System (OEMS) - Java Project Report.pdf
├── lib/                                  # Pre-Packaged Runtime Dependencies (FlatLaf, MySQL, OpenPDF, Webcam)
├── tools/                                # Offscreen Screenshot Capture & Rendering Utilities
├── run.bat                               # Windows Command Prompt One-Click Launcher
├── run.ps1                               # Native PowerShell One-Click Launcher
├── README.md                             # Project Documentation
└── LICENSE                               # MIT Open Source License
```

---

## 📂 Package Architecture (49 Java Classes)

| Package | Class Count | Architectural Responsibility | Key Design Patterns |
|:---|:---:|:---|:---|
| **`com.onlineexam.main`** | 1 | Application bootstrap, Look & Feel initialization, pre-flight checks, and EDT scheduling. | *Bootstrap Coordinator* |
| **`com.onlineexam.dao`** | 12 | Thread-safe JDBC persistence, PBKDF2 key stretching, session locking, proctoring persistence, and CTT analytics. | *DAO, Singleton, Factory, Service* |
| **`com.onlineexam.data`** | 4 | Immutable domain models, thread-safe in-memory state repository, answer evaluation, and vector PDF compilation. | *DTO, Value Object, Builder, Engine* |
| **`com.onlineexam.ui`** | 13 | Reusable UI design system tokens, glassmorphic containers, physics animations, and authentication views. | *Component, Composite, Observer* |
| **`com.onlineexam.ui.student`** | 9 | Candidate portal, assessment catalog, webcam consent, distraction-free kiosk exam runner, scorecards, and review. | *MVC View, State, Template Method* |
| **`com.onlineexam.ui.admin`** | 8 | Administrator command center, exam authoring, question bank management, psychometrics console, and proctor audit. | *Dashboard, TableRenderer, Observer* |
| **`com.onlineexam.test`** | 1 | Database network socket handshake and credential verification CLI utility. | *Diagnostic CLI* |

<details>
<summary><b>📋 Click to View the Complete 49-Class Inventory</b></summary>
<br/>

```
com.onlineexam.main
  └── Main.java
com.onlineexam.dao
  ├── DBConnection.java          ├── SchemaMigrator.java        ├── UserDAO.java
  ├── ExamDAO.java               ├── QuestionDAO.java           ├── AttemptDAO.java
  ├── SessionDAO.java            ├── SessionHeartbeat.java      ├── ProctorDAO.java
  ├── WebcamProctorService.java  ├── AchievementService.java    ├── CertificateService.java
  └── QuestionAnalyticsDAO.java
com.onlineexam.data
  ├── ExamConfig.java            ├── ExamStore.java
  ├── AnswerEvaluator.java       └── CertificatePdfBuilder.java
com.onlineexam.ui
  ├── UITheme.java               ├── Anim.java                  ├── GlassPanel.java
  ├── AuroraBackground.java      ├── AuthComponents.java        ├── DashboardComponents.java
  ├── PasswordStrengthMeter.java ├── ConfettiPanel.java         ├── RadarChartPanel.java
  ├── GlassDialog.java           ├── DemoFrame.java             ├── LoginUI.java
  └── SignupUI.java
com.onlineexam.ui.student
  ├── StudentDashboard.java      ├── SubjectSelectionUI.java    ├── InstructionsUI.java
  ├── ExamModule.java            ├── ResultUI.java              ├── ReviewUI.java
  ├── StudentPerformanceUI.java  ├── ProfilePanel.java          └── AchievementsPanel.java
com.onlineexam.ui.admin
  ├── AdminDashboard.java        ├── ExamManagementUI.java      ├── AddQuestionUI.java
  ├── ViewQuestionsUI.java       ├── PerformanceAnalysisUI.java ├── QuestionAnalyticsUI.java
  ├── ProctorLogUI.java          └── VerifyCertificateUI.java
Default Package
  └── TestDB.java
```

</details>

---

## 🛠️ Tech Stack & Dependencies

| Layer | Component | Version | Purpose |
|:---|:---|:---:|:---|
| **Core Runtime** | **Java SE (OpenJDK)** | `17+ / 21 LTS` | Object-oriented application logic, multithreaded concurrency |
| **UI Framework** | **Java Swing & Java2D** | Built-in | Window management, LCD sub-pixel font rendering, vector graphics |
| **Look & Feel** | **FlatLaf** | `3.5.x` | Modern light design tokens, rounded borders, glassmorphic cards |
| **Relational Database** | **MySQL Server (InnoDB)** | `8.0+` | Normalized relational storage, foreign keys, ACID transactions |
| **Database Driver** | **MySQL Connector/J** | `9.x` | High-performance Type-4 JDBC driver with batch execution |
| **Cryptography** | **Java Cryptography Architecture** | Built-in | PBKDF2WithHmacSHA256 stretching, 128-bit CSPRNG salts |
| **Document Engine** | **OpenPDF** | `1.3.40` | Archival vector PDF certificate generation |
| **QR Code Matrix** | **ZXing Core** | `3.5.3` | High-density 2D QR matrix generation and parsing |
| **Hardware Video** | **Webcam-Capture & BridJ** | `0.3.12` | Asynchronous webcam frame surveillance daemon |

---

## ⚡ Quick Start & Run Guide

### 📦 Standalone Release (Ready to Run)
1. Download the latest pre-packaged bundle: [**OnlineExamSystem-v1.1.0-Windows.zip**](https://github.com/navaneeth2205/Online-Exam-System/releases/download/v1.1.0/OnlineExamSystem-v1.1.0-Windows.zip)
2. Extract the archive into any folder.
3. Import `sql/database_setup.sql` into your local MySQL server (port 3306).
4. Double-click `run.bat` or `OnlineExamSystem.jar` to start!

---

### 🛠️ Developer Setup & Source Launch

#### 1. Prerequisites
- **JDK**: Java Development Kit 17 or higher (`java -version`).
- **MySQL**: MySQL Server 8.0 running on `localhost:3306`.

#### 2. Database Initialization
Execute the SQL setup scripts in MySQL Workbench or via CLI:
```bash
mysql -u root -p < sql/database_setup.sql
mysql -u root -p < sql/sample_data.sql
```

#### 3. One-Click Launch (Windows)

#### Native PowerShell:
```powershell
.\run.ps1
```

#### Windows Command Prompt:
```cmd
run.bat
```

> [!TIP]
> Both `run.ps1` and `run.bat` automatically detect if MySQL Server 8.0 is running on port 3306 and launch the local daemon in the background if needed.

#### Manual Compilation & Launch:
```powershell
# Compile all source files from java files/ into out/ directory
javac -cp "lib/*" -d out (Get-ChildItem -Path "java files" -Filter *.java -Recurse | Select-Object -ExpandProperty FullName)

# Verify database connection
java -cp "out;lib/*" TestDB

# Launch the Application
java -cp "out;lib/*" com.onlineexam.main.Main
```

---

## ☁️ Cloud Web Deployment (Render.com)

The project includes a ready-to-deploy **Docker + noVNC** configuration that streams the interactive Java Swing application directly to any web browser.

### 1-Click Setup on Render:
1. Fork or push this repository to GitHub.
2. Sign in to [Render.com](https://render.com) and click **New +** ➔ **Web Service**.
3. Select your repository `Online-Exam-System`.
4. Render will automatically detect `render.yaml` and select the **Docker** runtime.
5. Click **Deploy Web Service**.

Render will build the container, start the MariaDB database and virtual display (`Xvfb`), and provide a live public link (e.g., `https://online-exam-system-xxxx.onrender.com`) where the full application can be interacted with inside the browser without installing Java or MySQL locally.

---

<p align="center">
  <sub>Engineered in Core Java & MySQL • Released under the MIT License</sub>
</p>
