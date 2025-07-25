# Table Tracker System

This repository contains several versions of a Table Tracker System built with Python and Flask, providing real-time management of snooker and pool tables for gaming centers, clubs, and cafes. It supports desktop and mobile interfaces, session/bill tracking, price settings, user management, and more.

## Features

- **Real-Time Tracking:** Start, pause, and end sessions for each table, with timers and billing calculated automatically.
- **Snooker & Pool Support:** Manage multiple snooker and pool tables independently, each with customizable rates and session histories.
- **Session History:** Persistent session data for each table, including start/end time, amount, and date. Easily clear session data.
- **Rate Settings:** Change per-minute rates for each table (when idle) from a modern settings panel.
- **Split Bill:** Divide session amount among any number of players.
- **Mobile Interface:** Lightweight mobile web UI for remote table control.
- **User Management:** (Pro/Enhanced versions) Secure login system, admin/staff roles, add/remove users, role-based access.
- **Clean UI:** Modern, responsive UI with smooth scrolling, color-coded statuses, and easy navigation between Snooker and Pool.
- **Network Ready:** Access via local network IP; auto-opens on your browser.

## Getting Started

### Requirements

- Python 3.7+
- pip

### Installation

1. **Clone the repository:**
   ```sh
   git clone https://github.com/yourusername/weekwndrush.git
   cd weekwndrush
   ```

2. **Install dependencies:**
   ```sh
   pip install flask flask_cors flask_login werkzeug
   ```

3. **Run the application:**

   There are multiple versions/scripts. For the most feature-rich and production-ready version, use:

   ```sh
   python "Full working and ready to test table tracker.py"
   ```

   Or use other versions as needed (see below for script options).

4. **Access the app:**
   The terminal will print your local IP and URLs, e.g.:
   ```
   🖥️  Desktop Interface: http://192.168.1.100:8080
   📱 Mobile Interface: http://192.168.1.100:8080/mobile
   ```

   Open these URLs in your desktop or mobile browser on the same network.

## Script Overview

- **Full working and ready to test table tracker.py**  
  Professional business-ready solution with login, multi-user admin/staff roles, snooker & pool support, split bills, real-time updates, and user management.
  
- **Enhanced Complete Table Tracker System - With Login System, User Management & Remove Users.py**  
  Like above, but slightly simplified in features/roles.
  
- **Stable table tracker with split and UI.py**  
  Stable, modern UI, settings panel, no login system, useful for open environments.
  
- **Table tracker with pool and snooker server and stable ui final.py**  
  Includes improved pool section readability, dark theme for pool, per-table session history.
  
- **table_tracker_with_snooker_and_pool_table_data.py**  
  Home page navigation for both snooker and pool; both are active and fully functional.
  
- **table_tracker_snooker_and_Pool_Home_page.py**  
  Home page with game selection; pool section marked as "coming soon."
  
- **complete_table_tracker with setting for table price.py**  
  Adds per-table price settings and fixed scrolling.
  
- **complete_table_tracker copy.py**  
  Simple polling-based version for real-time updates.
  
- **complete_table_tracker with table data doen.py**  
  Adds persistent session data and clear buttons.

## Default Credentials (for login-enabled versions)

- **Admin:**  
  Username: `admin`  
  Password: `admin123`
- **Staff:**  
  Username: `staff1`  
  Password: `staff123`

## Customization

- **Number of Tables:**  
  Edit the relevant Python script(s) and modify the `self.snooker_tables` and `self.pool_tables` dictionaries as needed.
- **Pricing Options:**  
  Modify the `self.available_rates` list in each script.
- **Port:**  
  By default, the app runs on port 8080. Change the `port=8080` argument in the script to use another port.

## Security

- Passwords are hashed using Werkzeug.
- Only admin users can add/remove other users (in login-enabled versions).
- Do **not** use the default `SECRET_KEY` in production; update it in the script.

## Troubleshooting

- If the web UI doesn't open, check your firewall and make sure the chosen port (8080) is open.
- If running on a server or VM, make sure to use the correct local IP and that your device is on the same network.

## Contributing

Feel free to fork and contribute improvements! Open an issue or pull request for suggestions.

---

**License:** MIT  
**Author:** Hrishank21s  
