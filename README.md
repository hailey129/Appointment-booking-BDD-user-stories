# Appointment-booking-BDD-user-stories

# 📅 Online Appointment Booking – BDD User Stories

Welcome to a mini-case project designed to demonstrate my **Business Analyst** skills in writing user stories using the **BDD format (Given–When–Then)**. This system simulates an appointment booking process and shows how Agile-friendly documentation supports development teams and stakeholders.

## 💼 Project Overview

This project outlines the key user interactions of an appointment booking system, focusing on:

- 📌 Requirement gathering  
- ✍️ Writing user stories in BDD format  
- 🔁 Agile methodology alignment  
- 🧪 Supporting development and UAT

## 🧠 Business Context

A small service-based business (e.g., dental clinic or consulting firm) requires a digital system that allows customers to:

- Book, cancel, and reschedule appointments  
- Receive confirmations and reminders  
- Avoid booking conflicts


## 📋 BDD User Stories

### ✅ Booking an Appointment

```gherkin
Given a registered user is logged in  
When they select an available date and time  
Then the system should confirm the booking  
And send a confirmation email with details
```

### 📆 Viewing Appointments

```gherkin
Given the user is logged in  
When they navigate to “My Appointments”  
Then they should see a list of all upcoming appointments with date, time, and location
```

### 🔄 Rescheduling an Appointment
```gherkin
Given the user has a confirmed appointment  
When they select “Reschedule” and choose a new available time  
Then the appointment should be updated  
And a reschedule confirmation email should be sent
```

### ❌ Cancelling an Appointment
```gherkin
Given a user has an upcoming appointment  
When they click “Cancel” and confirm the cancellation  
Then the appointment should be removed from the system  
And the user should receive a cancellation email
```

### 🚫 Preventing Double Booking
```gherkin
Given another user has already booked a specific time slot  
When a user tries to book the same time slot  
Then the system should display an error saying “Time slot unavailable”
```

### ⏰ Sending Reminders
```gherkin
Given a user has a confirmed appointment within 24 hours  
When the time reaches 24 hours before the appointment  
Then the system should automatically send a reminder email or SMS
```

### 🚷 Handling No-Shows
```gherkin
Given a user fails to check in within 15 minutes of the appointment time  
When the system detects the missed appointment  
Then the appointment should be marked as “No Show”  
And a notification should be sent to the admin for follow-up
```

🔗 Portfolio Use
This project is designed to showcase:

- BDD user story writing for Agile development
- Requirements analysis for BA roles
- Clear stakeholder communication and system design thinking



