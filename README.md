# 🏥 HealthDesk - Patient Management System

A modern, full-stack healthcare management platform designed to eliminate long hospital wait times and streamline the entire patient journey. From registration to appointment scheduling and real-time SMS confirmations, HealthDesk solves a real-world problem that affects millions of patients every day.

Built with **Next.js 14, TypeScript, Appwrite, and Twilio**, this application delivers a seamless experience for patients while giving healthcare administrators powerful tools to manage appointments efficiently.

**🔗 Live Demo:** [hospital-one-hazel.vercel.app](https://hospital-one-hazel.vercel.app)

**🔑 Admin Access Passkey:** `111111`  
To access the admin dashboard, click the "Admin" link at the bottom of the homepage and enter the passkey above.

---

## ✨ Features

✅ **Patient Registration with Multi-Step Forms** - Comprehensive medical history, identification verification, and consent management.  
✅ **Appointment Booking System** - Patients can schedule appointments with their preferred doctor, pick a date and time, and provide their reason for visit.  
✅ **Admin Dashboard with Passkey Protection** - OTP-based admin access with client-side session persistence and server-side validation.  
✅ **Real-Time SMS Notifications** - Automated appointment confirmations and cancellation alerts powered by Twilio and Appwrite Messaging.  
✅ **Dynamic Status Management** - Admins can schedule, confirm, or cancel appointments with cancellation reason tracking.  
✅ **Secure File Upload** - Patients can upload identification documents stored securely via Appwrite Storage.  
✅ **Error Monitoring & Performance Tracking** - Integrated Sentry for production-grade error tracking, session replays, and performance insights.  
✅ **Fully Responsive Design** - Optimized for desktop, tablet, and mobile with a clean, modern dark mode UI.  
✅ **Type-Safe Architecture** - End-to-end TypeScript with Zod validation for bulletproof data integrity.

---

## 🔥 Tech Stack

### 🖥️ Frontend
- **Next.js 14** (App Router, Server Actions, Server Components)
- **TypeScript** for complete type safety
- **Tailwind CSS** for rapid, utility-first styling
- **ShadCN UI** for accessible, reusable components
- **React Hook Form + Zod** for robust form validation
- **React Datepicker** and **React Phone Number Input** for complex input handling

### 🔧 Backend & Services
- **Appwrite Cloud** (Authentication, Database, Storage, Messaging)
- **Twilio** (SMS delivery infrastructure)
- **Sentry** (Error monitoring and session replay)
- **Node Appwrite SDK** for server-side operations

### 🚀 DevOps & Deployment
- **Vercel** (Production hosting with CI/CD)
- **GitHub** (Version control)

---

## 🎯 The Problem It Solves

Booking and managing doctor appointments is often slow and unclear. Patients don’t always know if their request went through, and administrators end up handling everything manually across different tools.

HealthDesk simplifies this process with a clear registration and booking flow, real-time SMS confirmations, and a centralized admin dashboard to manage appointments efficiently. The result is better visibility, fewer missed appointments, and a smoother experience for both patients and staff.

---

## 🏗️ Architecture Highlights

### 🔐 Security
- Admin passkey gate with client-side session persistence and server-side validation
- Server-side validation with Zod schemas on every form submission
- Environment-based credential management
- Appwrite role-based permissions for fine-grained access control

### ⚡ Performance Optimized
- Server Actions eliminate API route boilerplate
- Next.js Image component for automatic optimization
- Path revalidation for instant admin dashboard updates after mutations
- Minimal client-side JavaScript with strategic server component usage

### 🧩 Reusable Component Library
- Custom form field system supporting 8+ input types (text, phone, date picker, select, checkbox, file upload, text area, and radio skeleton)
- Reduces form code from hundreds of lines to under 20 per field
- Fully extensible with strong TypeScript typing

### 📊 Smart Data Pipeline
- Aggregation logic for appointment statistics (scheduled, pending, cancelled counts)
- Single-query data fetching for admin dashboard
- Automatic path revalidation after appointment updates

---

## 📸 Screenshots

### **Patient Welcome Page**
The entry point where patients begin their registration journey.

<!-- UPLOAD SCREENSHOT HERE: Homepage showing CarePulse logo, "Hi there 👋", name/email/phone fields, Get Started button, and doctor image on the right -->
![Patient Welcome Page](your-image-url-here)

### **Multi-Step Registration Form**
Comprehensive patient information collection with personal, medical, and identification sections.

<!-- UPLOAD SCREENSHOT HERE: Registration page showing "Welcome 👋", Personal Information section with name/email/phone/date of birth/gender/address/occupation fields -->
![Registration Form - Personal Info](your-image-url-here)

<!-- UPLOAD SCREENSHOT HERE: Registration page scrolled down showing Medical Information section with primary physician dropdown, insurance fields, allergies, and medical history -->
![Registration Form - Medical Info](your-image-url-here)

<!-- UPLOAD SCREENSHOT HERE: Registration page scrolled down to Identification and Verification section with ID type dropdown, ID number, and file upload area -->
![Registration Form - Identification](your-image-url-here)

### **Appointment Booking Interface**
Doctor selection, date and time picker, and reason capture in a clean layout.

<!-- UPLOAD SCREENSHOT HERE: New Appointment page showing doctor dropdown, expected appointment date picker, appointment reason and comments/notes text areas, Submit Appointment button -->
![Appointment Booking](your-image-url-here)

### **Success Confirmation Page**
Elegant confirmation with appointment details and doctor information.

<!-- UPLOAD SCREENSHOT HERE: Success page showing "Your appointment request has been successfully submitted!" with the animated success badge, requested appointment details (doctor + date), and New Appointment button -->
![Success Confirmation](your-image-url-here)

### **Admin Passkey Modal**
OTP-based verification gate before accessing the admin dashboard.

<!-- UPLOAD SCREENSHOT HERE: Passkey modal on the homepage with "Admin Access Verification" title, 6 empty OTP slots, and "Enter Admin Passkey" button -->
![Admin Passkey Modal](your-image-url-here)

### **Admin Dashboard**
Real-time statistics cards with a paginated appointment data table.

<!-- UPLOAD SCREENSHOT HERE: Full admin dashboard showing "Welcome 👋", the 3 stat cards (Scheduled / Pending / Cancelled) with real numbers, and the data table below with patient rows, status badges, appointments, doctors, and Schedule/Cancel actions -->
![Admin Dashboard](your-image-url-here)

### **Schedule Appointment Modal**
Contextual form with pre-populated data for efficient admin workflows.

<!-- UPLOAD SCREENSHOT HERE: Schedule Appointment modal (after clicking Schedule action) showing the doctor dropdown pre-filled, date/time picker, reason, and notes fields -->
![Schedule Appointment Modal](your-image-url-here)

### **Cancel Appointment Modal**
Cancellation workflow with reason tracking.

<!-- UPLOAD SCREENSHOT HERE: Cancel Appointment modal showing the cancellation reason text area and red Cancel Appointment button -->
![Cancel Appointment Modal](your-image-url-here)

### **SMS Notification**
Real-time SMS confirmation delivered to the patient's phone.

<!-- UPLOAD SCREENSHOT HERE: Phone screenshot showing the received SMS from Twilio with the appointment confirmation text (doctor name + date + time) -->
![SMS Notification](your-image-url-here)

---

## 🚀 Why This Stands Out

HealthDesk is a production-grade application built with the same tools and patterns used by modern tech startups and enterprise engineering teams.

**What makes this project impressive:**

🔹 **Solves a real-world problem** that affects every person who has ever visited a hospital.  
🔹 **Full TypeScript coverage** from database schemas to React components.  
🔹 **Server Actions architecture** demonstrates understanding of the latest Next.js patterns.  
🔹 **Real SMS integration** via Twilio shows comfort with third-party APIs.  
🔹 **Production monitoring** via Sentry proves awareness of reliability concerns.  
🔹 **Complex forms done right** using a reusable field abstraction that scales to 20+ fields without code duplication.  
🔹 **Thoughtful UX details** like pre-filled default values when editing appointments, contextual button labels, and appropriate error messaging.

This project demonstrates full-stack proficiency, architectural thinking, and the ability to ship polished features that real users would actually rely on.

---

## 🧠 What I Learned Building This

Building HealthDesk taught me how to approach complex forms as a systems design problem rather than a UI problem. Once I built a single reusable CustomFormField component, adding new input types became trivial. That shift in thinking, from procedural UI to composable abstractions, has changed how I approach every project since.

I also learned how to integrate multiple third-party services (Appwrite, Twilio, Sentry) in a way that keeps each concern isolated. When Twilio fails, the app degrades gracefully. When Sentry captures an error, I can replay the exact session that caused it. These integration patterns are directly applicable to any production codebase.

---

## 📦 Getting Started Locally

### Prerequisites
- Node.js 18+
- npm or yarn
- Appwrite Cloud account
- Twilio account (for SMS)
- Sentry account (optional, for monitoring)

### Installation

```bash
git clone https://github.com/RelentlessCore/HealthDesk.git
cd HealthDesk
npm install
```

### Environment Variables

Create a `.env.local` file in the project root:

```env
NEXT_PUBLIC_ENDPOINT=https://cloud.appwrite.io/v1
PROJECT_ID=your_project_id
API_KEY=your_api_key
DATABASE_ID=your_database_id
PATIENT_COLLECTION_ID=patient
DOCTOR_COLLECTION_ID=doctor
APPOINTMENT_COLLECTION_ID=appointment
NEXT_PUBLIC_BUCKET_ID=your_bucket_id
NEXT_PUBLIC_ADMIN_PASSKEY=111111
SENTRY_AUTH_TOKEN=your_sentry_token
```

### Run the Development Server

```bash
npm run dev
```

Open [http://localhost:3000](http://localhost:3000) to see the app.

---

## 🎯 Future Enhancements

While HealthDesk is fully functional, there are several directions it could grow:

- **Dynamic doctor management** via an admin-controlled doctors collection
- **Patient-side appointment history** with cancellation and rescheduling
- **Multi-language support** for broader accessibility
- **Email notifications** as a backup to SMS
- **Analytics dashboard** showing booking trends and peak hours
- **Role-based admin access** with granular permissions per staff member

---

## 📬 Contact

Built by **Dardan Kabashi**

If you have feedback, questions, or want to collaborate, feel free to reach out. I'm always open to discussing new opportunities and projects.

---

Built for patients, designed for administrators, and engineered for scale. 🏥🚀
