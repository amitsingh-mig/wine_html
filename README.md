# EU–India Wine Summit 2026
## B2B Matchmaking & Pre-Scheduling System

An elegant, fully-featured frontend scheduling and registration system built for the **EU–India Wine Summit 2026** on the sidelines of SIAL Paris 2026. This repository connects public registrations, slot bookings, participant portals, and coordinator dashboards into a premium, cohesive workflow.

---

## 📂 Project Architecture

The system consists of the following key pages:

1.  **[index.html](index.html) (Homepage)**: The main event showcase introducing objectives, opportunity layers, programme schedules, and portal access points.
2.  **[register.html](register.html) (Registration)**: A premium registration form for participants to RSVP.
3.  **[Meeting_from.html](Meeting_from.html) (B2B Pre-Scheduler)**: Public step-by-step meeting request form where visitors submit profile details and select available 20-minute slots.
4.  **[user-login.html](user-login.html) (Participant Login)**: Access point for participants to log in and track their meeting request status.
5.  **[user-dashboard.html](user-dashboard.html) (Participant Dashboard)**: Schedule oversight where approved sessions highlight a download card and pending sessions are logged.
6.  **[admin-login.html](admin-login.html) (Admin Login)**: Access gate for organizers and event coordinators.
7.  **[dashboard.html](dashboard.html) (Organizer Dashboard)**: Central management dashboard to approve or decline slot requests, view stats, and inspect the B2B calendar timeline.
8.  **[style.css](style.css) (Global Stylesheet)**: The unified design system housing custom color variables, component parameters, and animations.

---

## ⚙️ Core System Workflows

### 1. **Slot Allocation & Availability**
*   Public requests default to `Pending` status.
*   Once an administrator approves a request in the Organizer Dashboard, its status changes to `Confirmed`.
*   Confirmed slots are dynamically synchronized with `localStorage` and become disabled/greyed out on the public booking scheduler, avoiding double bookings.

### 2. **Timeline Representation**
*   The admin dashboard features a horizontal chronological timeline grid from **09:00 AM to 05:00 PM** where confirmed meetings are plotted and staggered visually.

---

## 🔑 Test Credentials

For quick developer preview and testing, security gates are bypassed, and default credentials are set up:

### **Participant Login**
*   **Email**: `j.dupont@chateaumargaux.fr` *(or Priya Sharma `priya@sulavineyards.com`)*
*   **Password**: `password123`
*   *Note: Submitting any email in the public scheduler will automatically register a new user in localStorage with the default password `password123`.*

### **Organizer Login**
*   **Email**: `admin@mediaindia.eu`
*   **Password**: `admin123`

---

## 🎨 Design Tokens (Shared style.css)
*   **Cream/Paper background**: `#F5EEE6` / `#FBF7F1`
*   **Burgundy / Wine Accent**: `#8B1E3F`
*   **Wine Gold Accent**: `#C5A059`
*   **Typography**: Playfair Display (Serif headings) & Poppins/Inter (Body text)
