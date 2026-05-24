# ∞X - AI Creator Growth Platform

## Project Overview

Build a production-ready SaaS web application called ∞X.

∞X helps content creators improve their social media performance through analytics, growth recommendations, audience insights, engagement tracking, content strategy suggestions, and performance reporting.

---

## Tech Stack

### Frontend
- React 18
- TypeScript
- Vite
- Tailwind CSS
- React Router DOM
- React Query
- Recharts
- Framer Motion

### Backend
- Supabase

### Authentication
- Email/Password Authentication
- Google OAuth

### Database
- PostgreSQL via Supabase

### Storage
- Supabase Storage

### Hosting
- Vercel

---

## Design Requirements

Theme:
- Dark Theme

Colors:
- Background: #050816
- Surface: #0F172A
- Card: #111827
- Primary: #00BFFF
- Accent: #3B82F6
- Text: #FFFFFF
- Muted: #94A3B8

UI Requirements:
- Mobile First
- Fully Responsive
- SaaS Style
- Smooth Animations
- Clean Dashboard
- Premium Appearance

---

## Folder Structure

src/
├── components/
├── pages/
├── layouts/
├── hooks/
├── contexts/
├── services/
├── lib/
├── types/
├── utils/
├── constants/

---

## Pages

### Landing Page

Sections:
- Hero
- Features
- Benefits
- Testimonials
- Pricing
- FAQ
- CTA
- Footer

Headline:
Grow Faster. Create Smarter.

Subheadline:
AI-powered insights that help creators increase engagement, reach, and audience growth.

Buttons:
- Start Free
- View Demo

---

### Authentication

Pages:
- Login
- Signup
- Forgot Password
- Reset Password

Features:
- Email Login
- Google Login
- Protected Routes
- Session Persistence

---

### Dashboard

Widgets:
- Growth Score
- Engagement Rate
- Followers Growth
- Audience Insights
- Content Performance
- Recent Activity
- Notifications

Sidebar:
- Dashboard
- Analytics
- Profile
- Settings

---

### Analytics

Charts:
- Growth Trend
- Engagement Trend
- Reach Trend

Metrics:
- Total Posts
- Total Engagement
- Average Engagement Rate
- Growth Percentage

Use Recharts.

---

### Profile

Features:
- Update Username
- Upload Avatar
- Change Password
- Edit Profile

---

### Settings

Sections:
- General
- Notifications
- Privacy
- Subscription

Danger Zone:
- Delete Account

---

## Database Schema

### profiles

id UUID PRIMARY KEY
email TEXT UNIQUE
username TEXT
avatar_url TEXT
created_at TIMESTAMP

### analytics

id UUID PRIMARY KEY
user_id UUID
metric_name TEXT
metric_value NUMERIC
created_at TIMESTAMP

### activities

id UUID PRIMARY KEY
user_id UUID
activity_type TEXT
activity_description TEXT
created_at TIMESTAMP

### notifications

id UUID PRIMARY KEY
user_id UUID
title TEXT
message TEXT
is_read BOOLEAN
created_at TIMESTAMP

---

## Row Level Security

Users may:
- Read own data
- Update own data
- Delete own data

Users may not:
- Access another user's data

Generate all RLS policies.

---

## Supabase Setup

Create:

src/lib/supabase.ts

Environment Variables:

VITE_SUPABASE_URL=
VITE_SUPABASE_ANON_KEY=

Implement:
- Authentication
- Database Access
- Storage Uploads
- Session Management

---

## Security

- Form Validation
- Input Sanitization
- Error Boundaries
- Loading States
- Toast Notifications
- Secure Sessions

---

## Deliverables

Generate:

- Complete React Application
- TypeScript Types
- Components
- Pages
- Layouts
- Supabase Integration
- SQL Schema
- RLS Policies
- Authentication Flow
- Dashboard
- Analytics Charts
- Responsive Design
- Vercel Deployment Config
- README
- .env.example

Code must be production-ready, scalable, clean, and fully typed.
# -Max-X
