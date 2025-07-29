# Hospital-dashboard
Project Overview
The Hospital Doctor Dashboard is a powerful tool designed to simplify hospital operations, combining real-time visualization for doctors, patients, billing, and appointments. It is fully integrated with a robust backend based on MySQL views for medical, staff, and financial management.

Features
1. Doctor Dashboard
Doctor Profiles: View doctor details, specializations, availability, ratings, and manage schedules.
Appointment Management: List all upcoming appointments for seamless workflow.
Patient Monitoring: See real-time patient status (admitted/discharged) alongside financials.
Commission & Billing Analytics: Track doctor-wise commission, total bills, and financial performance.
Graphical Widgets: Interactive graphs, sliders, and tables for quick insights.

2. Patient, Financial, and Stock Insights
Patient Tracking: Comprehensive patient records including status, gender, admission/discharge dates, and billing.
Automated Financials: Calculate commissions, totals, and breakdowns at a glance.
Inventory Overview: Monitor medical stock, reorder levels, expiry, and vendor information.
Tech Stack

Frontend: power bi 

Backend: MySQL (using advanced SQL Views from provided scripts)
APIs: RESTfulPower bi recommended for connecting frontend with database

Database Schema & Views
Predefined SQL Views
Provided in /mysql.sql file (see attachment):

medical_stock_info

Joins medicine stock with supplier details for inventory snapshots.
hospital_patient_details
Aggregates patient, doctor, surgery, bed, room, billing, and satisfaction info in one comprehensive view.

Note: Ensure all referenced tables (patient, doctor, beds, hospital_bills, etc.) exist with necessary columns/constraints.

Installation & Setup
1. Database Setup
Import the SQL views from the mysql.sql file into your MySQL database:

bash
mysql -u username -p hospital_db < mysql.sql
Validate all required base tables exist and are populated.

2. Frontend Setup (Sample: React)
Clone your repo

Usage Guide
Login: Authenticate as a doctor, admin, or staff.

Doctor List: Browse doctors, filter by specialization or name, and check status.

Appointments: See and schedule patient visits; upcoming appointments are displayed in an organized format.

Patient Records: Track patient status, billing, and live bed occupancy.

Financial Analytics: Instantly analyze earnings, commission rates, and hospital revenue.

Stock Management: Use the inventory view for monitoring low stock and upcoming expiries.

Customization & Extensions
Add custom charts for department-wise analytics or historical patient trends.

Integrate with hospital notification/email systems for automated alerts.

Extend database views to include additional business logic (insurance, custom billing, or audit logs).

Implement role-based access control for enhanced security.

Best Practices
Data Security: Apply access controls at both the database and application levels.

Performance: Index key columns; optimize SQL for large datasets.

Data Accuracy: Implement validation on entry and regular audits.

Scalability: Modularize frontend and backend for easy scaling.

Contributing
Fork the repository and open pull requests for improvements or bug fixes.

Suggest new features or report bugs via the issue tracker.

License
This project is open for educational, research, and prototyping purposes. For commercial use, review all third-party dependency licenses.

Contact
For implementation help, feedback, or queries:

Email: [mrsuhail052099@gmail.com]
[Suhail Khan]
