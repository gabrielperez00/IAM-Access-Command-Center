# Technical Room Access Log
### Secure Identity-Based Entry System

I developed this application to replace manual tracking methods with a secure, automated digital log. This project demonstrates how to use identity-based logic to manage facility access and maintain a clean audit trail for security compliance.

### Technical Implementation

* **Identity-Gated Access:** The app utilizes the Microsoft 365 login token to identify users automatically. This ensures all check-in data is tied to a verified identity without requiring manual input.
* **Administrative Security:** I implemented a visibility rule that checks the user's email against an authorized list. If a user is not an administrator, the settings and historical data logs are completely hidden from their view.
* **Real-Time Data Management:** Using Power Fx Patch functions, the app manages a live "Check-In/Check-Out" lifecycle. It updates existing database records in real-time to reflect when a user has departed the room.
* **Dynamic Filtering:** The "Active Roster" view is engineered to only show current occupants. I built a custom toggle for the Admin view that allows a supervisor to switch between "Live" and "All History" views instantly.

### Stack
* **Platform:** Microsoft Power Apps
* **Identity:** Entra ID (Azure AD)
* **Backend:** SharePoint / Dataverse
* **Logic:** Power Fx
