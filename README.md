# BoomRec Recruitment Web Platform

A professional, responsive web platform designed for **BoomRec Recruitment** to showcase workforce and HR solutions while facilitating talent acquisition through an integrated job board.

---

## 📁 Project Details

* **Project Name:** Intelligent Outsourcing & HR Platform
* **Academic Institution:** Cairo University - Faculty of Graduate Studies for Statistical Research
* **Degree:** Master of Software Engineering 2025-2026
* **Student Name:** Walid Moheyeldin
* **Student Number:** 202301526
* **Supervisor:** Dr. Maged Mamdouh

---

## 🚀 Features

### **Public-Facing Website**
* **Informational Pages:** Includes comprehensive static content for Home, About Us, Services (Recruitment, Payroll, HR Outsourcing, Personnel Administration, Training), and Contact sections.
* **Job Board:** A dynamic module where anonymous users can browse open vacancies and apply directly.
* **Lead Generation:** Implementation of a job application system to capture candidate data and notify the BoomRec team in real-time.

### **Administrative Dashboard**
* **Job Management (Admin):** Secure dashboard to Create, Read, Update, and Delete (CRUD) job postings.
* **Applicant Tracking:** Centralized storage of all applicant data for administrative review.
* **Notification System:** Automatic email alerts to the Admin upon new applications.

---

## 🛠️ Technical Stack

| Component | Technology |
| :--- | :--- |
| **Framework** | ASP.NET Core MVC (Latest Version) |
| **Database** | SQL Server (Job postings and applicant data) |
| **Frontend** | HTML5, CSS3, JavaScript (Responsive Design) |
| **Security** | ASP.NET Core Identity for secure admin access |
| **Communication** | SMTP integration for automated email notifications |
| **Hosting** | Docker or IIS |

---

## 🏗️ Solution Architecture

The solution utilizes a single-node architecture optimized for the project's current small-scale requirements:

* **Web Server:** Docker Compose that includes 3 containers or IIS on a single shared Windows Server node hosts the application logic.
* **Data Layer:** SQL Server manages both job postings and applicant data on the same node.
* **Notification Flow:** Applications trigger an SMTP relay using customer-provided credentials to notify the HR team.

---

## ⚙️ Configuration & Assumptions

* **Infrastructure:** The project is currently small-scale and does not require High Availability (HA) or complex horizontal scalability at this stage.
* **Email Configuration:** The customer provides a dedicated email account and SMTP settings for system notifications.
* **Content:** All static website content, branding, and the logo are provided by the client and integrated as final assets.

---

## 🛠️ Getting Started

1. **Clone the Repository:**
   ```
   git clone https://github.com/WalidMoheyEldin/BoomRec.git
2. **Launch the platform:**
    ```
    docker-compose up -d --build
3. **Access URLs:** 
    - Main Website: http://localhost:5440
    - Control Center (Admin): http://localhost:5441
4. 🔐 **Credentials & Evaluation Data** <br />
The deployment is pre-seeded with sample data for demonstration:

| Role | Username | Password |
| :--- | :--- | :--- |
| Admin | admin@boomreceg.com | P@$$w0rd |

## ⏳ Trial & Evaluation License

**BoomRec** is provided with a **30-Day Trial License** to allow for a comprehensive evaluation of its features. 

* **Trial Activation:** The 30-day period begins automatically upon the first initialization of the system's data.
* **Evaluation Period:** Users have full access to all platform modules, including the AI-enhanced recruitment tools and the administrative dashboard, for the duration of the trial.
* **Post-Trial:** After the 30-day period, the system transitions into a "Secure-Lock" state to protect trial terms and data integrity.