
# InternSync: Revolutionizing Internship Management

## Table of Contents
- [Introduction](#introduction)
- [The Problem](#the-problem)
- [Existing Systems](#existing-systems)
- [Proposed Solution: InternSync](#proposed-solution-internsync)
- [Key Features](#key-features)
- [Technical Overview](#technical-overview)
- [Conclusion](#conclusion)
- [Acknowledgements](#acknowledgements)

## Introduction
Internships are a critical bridge between academic learning and real-world experience, especially during the eighth semester of a student's education. However, managing internships has traditionally been a cumbersome process, often relying on outdated methods that hinder effective communication and oversight.

## The Problem
The current landscape of internship management is riddled with challenges:
- **Inefficient Communication**: Interns often lack timely feedback from mentors, leading to confusion and isolation.
- **Manual Processes**: Reliance on spreadsheets and paper-based reports creates inefficiencies and increases the administrative burden.
- **Lack of Accountability**: Tracking intern progress is cumbersome, resulting in delays in feedback and oversight.

## Existing Systems
Traditional internship management systems are fragmented and disconnected, relying heavily on manual processes. This leads to:
- Delays in feedback and guidance for interns.
- Ineffective tracking of intern activities.
- A lack of a centralized platform for communication among stakeholders.

## Proposed Solution: InternSync
InternSync is a comprehensive web and mobile platform designed to streamline the management and tracking of internship activities. By automating and centralizing the internship management process, InternSync enhances communication and oversight for all parties involved.

### Key Features
- **Centralized Management**: Automates daily report submissions and provides analytics dashboards for performance monitoring.
- **Hierarchical Access**: Role-based access for interns, college mentors, company mentors, and administrators ensures efficient management.
- **Key Modules**:
  - **Attendance Management**
  - **Daily Report Submission**
  - **Internship Management**
  - **Mentor Assignment**
- **Mobile Application**: Offers seamless access to all functionalities for students and mentors.

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
| PostgreSQL | Relational database for data management |

### Hardware Requirements
| Provider       | CPU                | Memory (RAM) | Storage                   | Bandwidth     |
|----------------|--------------------|---------------|---------------------------|---------------|
| Vercel         | Virtual CPUs (auto-scaled) | Up to 4GB    | Ephemeral storage for serverless functions | 100 GB/month  |
| Supabase       | Virtual CPUs (auto-scaled) | Dynamic memory allocation | 500 MB database storage | 2 GB/month    |

## Getting Started

First, run the development server:

```bash
npm run dev
# or
yarn dev
# or
pnpm dev
# or
bun dev
```

Open [http://localhost:3000](http://localhost:3000) with your browser to see the result.

You can start editing the page by modifying `app/page.tsx`. The page auto-updates as you edit the file.

This project uses [`next/font`](https://nextjs.org/docs/basic-features/font-optimization) to automatically optimize and load Inter, a custom Google Font.

## Learn More

To learn more about Next.js, take a look at the following resources:

- [Next.js Documentation](https://nextjs.org/docs) - learn about Next.js features and API.
- [Learn Next.js](https://nextjs.org/learn) - an interactive Next.js tutorial.

You can check out [the Next.js GitHub repository](https://github.com/vercel/next.js/) - your feedback and contributions are welcome!

## Deploy on Vercel

The easiest way to deploy your Next.js app is to use the [Vercel Platform](https://vercel.com/new?utm_medium=default-template&filter=next.js&utm_source=create-next-app&utm_campaign=create-next-app-readme) from the creators of Next.js.

Check out our [Next.js deployment documentation](https://nextjs.org/docs/deployment) for more details.
