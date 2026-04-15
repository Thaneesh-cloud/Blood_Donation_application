# Blood Connect — Blood Donation Web Platform

A full-stack web application built with Django that connects blood donors
with recipients in real time. Developed as a group project for CIS5898
at Florida Institute of Technology (Fall 2024).

## Overview

Blood Connect addresses the critical challenge of matching blood donors
with recipients quickly and accurately. The platform supports real-time
blood availability tracking, automated blood type matching, emergency
request alerts, and map-based donation center discovery.

## Features

### Core Functionality
- **Donor & Recipient Registration** — users sign up as donors or recipients with blood type, location, and contact details
- **Automated Blood Type Matching** — real-time compatibility check between recipients and available donors
- **Blood Inventory Tracking** — live blood stock levels across nearby donation centers
- **Emergency Request System** — recipients can trigger urgent alerts that notify nearby compatible donors instantly
- **Map Integration (Leaflet.js)** — locate nearby blood donation centers and camps on an interactive map
- **Donation Points System** — donors earn points per donation, visible on their profile dashboard
- **Admin Dashboard** — admins manage blood inventory, user accounts, and delivery coordination

### User Roles
| Role | Capabilities |
|------|-------------|
| Donor | Register, view nearby centers, make donations, earn points |
| Recipient | Search blood types, request blood, trigger emergency alerts |
| Admin | Manage inventory, oversee requests, coordinate deliveries |

## Tech Stack

| Layer | Technology |
|-------|-----------|
| Backend | Django (Python) |
| Database | SQLite3 |
| Frontend | HTML, CSS, JavaScript |
| Map Integration | Leaflet.js |
| Real-time Updates | REST API |
| Version Control | Git / GitHub |

## Application Flow

1. User registers as donor or recipient
2. Donor logs in → sees nearby donation centers + current blood stock
3. Recipient searches for blood type → submits request
4. System runs real-time blood type compatibility matching
5. In emergencies → recipient triggers urgent request → nearby donors are alerted
6. Donation confirmed → inventory updated → recipient notified

## Project Structure

```
blood_connect/
├── accounts/          # User auth, registration, roles
├── donors/            # Donor profiles, donations, points
├── recipients/        # Blood requests, emergency alerts
├── inventory/         # Real-time blood stock management
├── admin_panel/       # Admin controls and dashboard
├── templates/         # HTML templates
├── static/            # CSS, JS, Leaflet.js assets
└── manage.py
```

## Setup Instructions

```bash
# Clone the repo
git clone https://github.com/your-username/blood-donation-app.git
cd blood-donation-app

# Install dependencies
pip install -r requirements.txt

# Run migrations
python manage.py migrate

# Start the development server
python manage.py runserver
```

## Key Concepts Demonstrated

- Django MVT (Model-View-Template) architecture
- Role-based access control (RBAC) — donor, recipient, admin
- Real-time data management via REST API
- Geolocation integration with Leaflet.js
- Emergency alert and notification system
- Object-oriented design (class and sequence diagrams)

## Author

Thaneesh Perabathula
M.S. Computer Information Systems — Florida Institute of Technology
