
# InternSync : Internship Activity Monitoring Portal

## Table of Contents
- [Introduction](#introduction)
- [Key Features](#key-features)
- [Technical Overview](#technical-overview)
- [Installation](#installation)

## Introduction
Internsync is a web platform designed to streamline the management and tracking of internship activities for interns, college mentors, and company mentors during the eighth
semester. It replaces traditional Excel-based systems by centralizing the submission and review of daily reports, allowing interns to submit their internship details and daily progress directly through the platform. College mentors benefit from automated weekly performance summaries via analytics dashboards, enabling continuous monitoring and feedback.

### Key Features
- **Centralized Management**: Automates daily report submission process and provides analytics dashboards for performance monitoring.
- **Hierarchical Access**: Role-based access for interns, college mentors, company mentors, and administrators ensures efficient management.
- **Key Modules**:
  - **Attendance Management**
  - **Daily Report Submission**
  - **Internship Management**
  - **Mentor Assignment**

## Technical Overview
InternSync leverages modern web technologies to provide a robust solution:
- **Frontend**: Built using **Next.js** and **TypeScript** for a dynamic user experience.
- **Backend**: Utilizes **Supabase** for real-time capabilities and PostgreSQL for data management.
- **Deployment**: Hosted on **Vercel**, ensuring fast and reliable performance.

### Software Requirements
| Technology | Description |
|------------|-------------|
| Next.js    | React framework for building web applications |
| TypeScript | Typed JavaScript for better tooling |
| Supabase   | Backend as a Service for real-time capabilities |


### Hardware Requirements
| Provider       | CPU                | Memory (RAM) | Storage                   | Bandwidth     |
|----------------|--------------------|---------------|---------------------------|---------------|
| Vercel         | Virtual CPUs (auto-scaled) | Up to 4GB    | Ephemeral storage for serverless functions | 100 GB/month  |
| Supabase       | Virtual CPUs (auto-scaled) | Dynamic memory allocation | 500 MB database storage | 2 GB/month    |

## Installation
To set up the project locally, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/Swaraj2004/internsync.git
   cd intern-sync
   ```

2. **Install dependencies**:
   For the web application:
   ```bash
   cd web
   npm install
   ```
3. Set up Supabase
   
   - Create a Supabase Account : 
     - Go to Supabase and sign up for a free account.
     - Create a new project in your dashboard.

   - Add Email Providers (SMTP) :
        In Supabase, go to Authentication > Settings > Email provider and configure your SMTP details.
  
   - Update Email Templates :
     - Customize email templates under Authentication > Templates in Supabase as needed.
     - List of Email templates to change
       - Confirm signup
       - Invite user
       - Reset password  
  
   - Configure URL Settings :
        In Settings > Site URL, add the below url for local development.
     - Site URL
       - http://localhost:3000
     - Redirect URLs
       - http://localhost:3000/set-password
       - http://localhost:3000/update-password
       - http://localhost:3000/verify-email
  
   - Add SQL Queries and Functions :
     - In the SQL Editor in Supabase, add the necessary SQL queries and functions.
     - Run each script directly in the editor.
     - Note : The Supabase Functions are provided in the repository folder at ![supabase/sql](https://github.com/Swaraj2004/supabase/sql)

4. **Set up environment variables**:
   Create a `.env.local` file in the web directory and add your Supabase credentials:
   ```
   NEXT_PUBLIC_SUPABASE_URL=your_supabase_url
   NEXT_PUBLIC_SUPABASE_ANON_KEY=your_supabase_anon_key
   SUPABASE_SERVICE_ROLE_KEY=your_supabase_service_role_key
   NEXT_PUBLIC_URL=http://localhost:3000
   SMTP_USER=your_smtp_email
   SMTP_PASSWORD=your_smtp_app_password
   ```

5. **Run the application**:
   For the web application:
   ```bash
   npm run dev
   ```


6. Open [http://localhost:3000](http://localhost:3000) on your browser to see the result.
