# Job Application Tracker

A web-based application to help students and professionals organize and manage job applications, contacts, interviews, and follow-ups. Built with **PHP**, **MySQL**, **AJAX**, **JavaScript**, and **CSS**.

## Overview
The project centralizes all job-related data into one place. Users can create and manage applications, track status updates, add notes, set reminders, and maintain a company directory. The site is dynamic and interactive, with client–server communication handled via AJAX returning JSON responses.

## Features (Planned)
- **Create Job**: Add a new job entry with role, company, link, status, and important dates.  
- **Update Status**: Progress applications through stages (new, applied, phone screen, interview, offer, rejected).  
- **Notes**: Attach notes to each job.  
- **Search, Filter, Sort**: Quickly find applications by keyword, company, status, or date.  
- **Reminders**: Set follow-ups or snooze actions, with dashboard notifications.  
- **Company Directory**: Manage company details including industry, location, and contacts.  
- **Delete**: Remove jobs or notes with confirmation.  
- **Authorization**: Register/login with sessions and password hashing.  

## Tech Stack
- **Frontend**: HTML, CSS, JavaScript (AJAX interactivity)  
- **Backend**: PHP (server endpoints returning JSON)  
- **Database**: MySQL (job records, notes, company info, user accounts)  

## Database Schema
The schema is provided in [`jobapp_tracker.sql`](./jobapp_tracker.sql).  
Import it into MySQL before running the project.

### Tables include:
- users (authentication and sessions)
- jobs (job applications and status)
- notes (user notes tied to jobs)
- companies (company directory)
- supporting indexes for search and filtering

## Requirements
- PHP 8+  
- MySQL 8+  
- Web server (Apache or similar with PHP support)

## Project Status
🚧 Work in progress. Database schema completed. Next milestones: API endpoints, frontend integration.

## How to Run (once implemented)
```bash
git clone https://github.com/<your-username>/job-application-tracker.git
cd job-application-tracker
mysql -u <user> -p < jobapp_tracker.sql
# Configure database credentials in config.php.
php -S localhost:8000
# Open http://localhost:8000 in your browser.

---

## License
MIT License – see [LICENSE](LICENSE) for details.
