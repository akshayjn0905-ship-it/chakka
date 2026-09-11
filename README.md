<img width="1280" height="640" alt="git (1)" src="https://github.com/user-attachments/assets/8920b256-2ba8-4988-b824-5351134eb4bd" />



# UDAYIPP CELER


## Basic Details
### Team Name: [Team Vaah]


### Team Members
- Team Lead: [Akshay J Nair] - [Sahrdaya College of Engineering and Technology]
- Member 2: [Adithya P] - [Sahrdaya College of Engineering and Technology]


### Project Description
[A completely legitimate-looking University Academic Services Portal designed to provide students with everything they could possibly need — study materials, homework, assignments, research, results, and more.

Except... almost none of it is actually academic. Most buttons secretly redirect students to completely unrelated websites, while the one button that looks like a break launches a mandatory 25-minute focus session.]

### The Problem (that doesn't exist)
[Students have too much freedom when using university portals.

They can click whatever they want, leave whenever they want, procrastinate whenever they want, and — most importantly — they can actually expect buttons to do what they say.

We decided this was a serious problem that absolutely needed solving.]

### The Solution (that nobody asked for)
[We created a fake university portal packed with convincing academic services.

"Study Materials" → Rickroll
"Homework Centre" → YouTube Trending
"Assignments" → Instagram Explore
"Project Workspace" → GitHub Explore
"Academic Results" → Wikipedia
"Exam Preparation" → Coursera
"Campus News" → Reddit News
"Study Audio" → Spotify Study
"Student Community" → Discord
Search → Google

And then there's "Let's Chill".

Clicking it launches a fullscreen focus environment with a 25-minute Pomodoro timer, a productivity checklist, and absolutely no chill.

Leaving fullscreen triggers an interruption warning, and the secret escape key is Y. The focus session can also be completed normally after the 25-minute timer finishes.]

## Technical Details
### Technologies/Components Used
For Software:
HTML5
CSS3
JavaScript
Browser Fullscreen API
JavaScript DOM manipulation
setInterval() for the Pomodoro timer
External website redirects

For Hardware:
No additional hardware required
Any computer/laptop with a modern web browser

### Implementation
For Software:
The project is implemented as a single HTML webpage containing:

University-style dashboard UI
Sidebar navigation
Academic service cards
Loading animations before redirects
External website redirections
Search functionality
Fullscreen focus mode
25-minute Pomodoro timer
Focus checklist
Fullscreen-exit detection
Secret keyboard exit using the Y key
Session completion screen

The portal's service buttons use JavaScript functions to redirect users to different external websites after displaying a fake loading screen.
# Installation
[No installation or external dependencies are required.

Download or clone the repository.
Open the HTML file in a modern web browser.]

# Run
[Simply open the .html file in:

Google Chrome
Microsoft Edge
Firefox
Any modern browser supporting the Fullscreen API]

### Project Documentation
For Software:
# University Academic Services Portal 🎓

## 1. Project Overview

The **University Academic Services Portal** is a web-based student dashboard designed to look like a professional university academic management system.

The portal provides a realistic-looking interface containing academic statistics, student services, deadlines, notifications, external resources, and a dedicated focus/study mode.

However, the project also includes a humorous twist: several academic service buttons redirect users to unrelated external websites, creating a **prank-style experience**. The main exception is the **"Let's Chill"** service, which opens a fullscreen focus environment with a 25-minute Pomodoro timer.

The project is built entirely using **HTML, CSS, and JavaScript**, with no backend or database.

---

## 2. Objectives

The main objectives of the project are:

* To create a realistic university student dashboard.
* To demonstrate modern HTML and CSS interface design.
* To implement interactive elements using JavaScript.
* To demonstrate event handling and browser APIs.
* To create a functional Pomodoro-style focus timer.
* To implement fullscreen mode and fullscreen interruption detection.
* To combine a professional-looking interface with humorous/prank interactions.
* To demonstrate how a simple frontend application can create an engaging user experience.

---

## 3. Technologies Used

### HTML5

Used to create the structure and content of the portal.

### CSS3

Used for:

* Layout
* Colors
* Typography
* Cards
* Buttons
* Responsive design
* Animations
* Fullscreen overlays
* Hover effects

### JavaScript

Used to provide interactivity and application functionality, including:

* External website redirection
* Loading screens
* Search functionality
* Fullscreen control
* Keyboard event handling
* Pomodoro timer
* Session completion
* Dynamic date display

---

## 4. Main Features

### 4.1 Student Dashboard

The main dashboard presents a university-style student information system.

It contains:

* Sidebar navigation
* Search bar
* Notification indicator
* Student profile
* Welcome section
* Academic statistics
* Academic services
* Upcoming deadlines
* Portal notifications
* Footer information

The dashboard uses a fixed sidebar and responsive content layout.

---

### 4.2 Academic Statistics

The dashboard displays four sample academic statistics:

* Attendance: **87%**
* Assignments: **06**
* Academic Score: **8.6**
* Deadlines: **04**

These are presented using separate statistic cards for a clean dashboard-style appearance.

---

### 4.3 Academic Services

The portal contains 12 service cards:

1. Study Materials
2. Homework Centre
3. Assignments
4. Project Workspace
5. Academic Calendar
6. Study Audio
7. Research Database
8. Academic Results
9. Exam Preparation
10. Student Community
11. Campus News
12. Let's Chill

Each service has an icon, service code, description, and action button.

---

## 5. Prank / Redirect System

The project uses JavaScript functions to make the service buttons appear as though they are connecting to university systems.

Before opening the destination, a loading screen is displayed for approximately **900 milliseconds**.

The common `redirectWithLoading()` function controls this behavior.

Examples include:

* Study Materials → YouTube video
* Homework Centre → YouTube Trending
* Assignments → Instagram Explore
* Project Workspace → GitHub Explore
* Academic Calendar → Google Calendar
* Study Audio → Spotify Study
* Research Database → Google Scholar
* Academic Results → Wikipedia
* Exam Preparation → Coursera
* Student Community → Discord
* Campus News → Reddit News

These destinations are deliberately used as part of the humorous concept of the project.

---

## 6. Search Function

The dashboard contains a search field labelled:

> "Search academic services..."

When the user enters a search query and presses **Enter**, JavaScript captures the input and opens a Google search using the entered query.

The query is processed using `encodeURIComponent()` so that it can safely be included in the search URL.

---

## 7. Let's Chill — Focus Mode

The **Let's Chill** button is the main functional feature of the project.

Instead of opening a normal external website, it launches a dedicated **Student Focus Environment**.

The focus screen contains:

* Focus Mode Active indicator
* 25-minute timer
* Start Focus button
* Reset Timer button
* Focus checklist
* Motivational message
* Fullscreen mode

The focus environment is displayed separately from the main dashboard.

---

## 8. Pomodoro Timer

The focus mode implements a 25-minute countdown timer.

The timer starts with:

**1500 seconds = 25 minutes**

JavaScript stores the remaining time in the `seconds` variable and uses `setInterval()` to decrease it once every second.

### Timer Controls

#### Start Focus

The `startTimer()` function:

1. Checks whether a timer is already running.
2. Starts a one-second interval.
3. Decreases the remaining seconds.
4. Updates the timer display.
5. Completes the session when the timer reaches zero.

#### Reset Timer

The `resetTimer()` function:

* Stops the current timer.
* Resets the timer to 1500 seconds.
* Updates the display back to `25:00`.

---

## 9. Focus Checklist

The focus screen includes a checklist containing five tasks:

* Review today's class notes
* Complete pending homework
* Revise important formulas
* Practice examination questions
* Prepare tomorrow's study plan

This gives the focus screen an additional productivity-oriented function.

---

## 10. Fullscreen Focus Mode

When Focus Mode is activated, the application attempts to enter the browser's fullscreen mode using:

`document.documentElement.requestFullscreen()`

The page also disables normal body scrolling while the focus screen is active.

---

## 11. Fullscreen Interruption Detection

The application monitors the browser's `fullscreenchange` event.

If the user exits fullscreen while Focus Mode is active, the application detects the change and displays a **"Focus Mode Interrupted"** warning.

The user can then return to fullscreen using the provided button.

This demonstrates the use of browser events and the Fullscreen API.

---

## 12. Secret Exit Key

The project includes a hidden keyboard shortcut.

While Focus Mode is active:

**Y / y → Exit Focus Mode**

A global keyboard event listener detects the key press and calls the `secretExit()` function.

The exit function:

* Disables focus mode
* Hides the study screen
* Hides the warning
* Restores page scrolling
* Exits browser fullscreen

This adds an additional humorous element to the application.

---

## 13. Session Completion

When the 25-minute timer reaches zero, the `completeSession()` function is called.

It:

* Stops the timer
* Disables focus mode
* Allows normal exiting
* Displays the session completion screen

The completion screen congratulates the user for completing the focus session and provides an exit button.

---

## 14. Dynamic Date

The dashboard automatically generates the current date using JavaScript's `Date` object.

The date is formatted using the `en-IN` locale and displays:

* Weekday
* Day
* Month
* Year

This prevents the displayed date from being permanently fixed in the source code.

---

## 15. Responsive Design

The website includes CSS media queries to make the interface adapt to different screen sizes.

### Medium Screens

At widths below 1000px:

* Sidebar becomes smaller.
* Statistics use two columns.
* Services use two columns.

### Mobile Screens

At widths below 700px:

* Sidebar is hidden.
* Main content occupies the full width.
* Statistics become a single column.
* Services become a single column.
* Lower dashboard sections become a single column.
* Timer font size is reduced.

This makes the application usable across desktop, tablet, and mobile screen sizes.

---

## 16. User Interface Design

The interface follows a professional university-management-system aesthetic.

### Main Design Characteristics

* Dark navy sidebar
* White content cards
* Light grey background
* Blue accent colors
* Green focus-mode elements
* Rounded cards
* Subtle borders
* Hover animations
* Responsive grid layouts

The service cards use hover transformations and shadows to provide visual feedback when the user interacts with them.

---

## 17. Project Workflow

The basic workflow of the application is:

```text
Open Website
     ↓
University Dashboard
     ↓
Select Academic Service
     ↓
 ┌─────────────────────────────┐
 │                             │
External Service          Let's Chill
 │                             │
 ↓                             ↓
Loading Screen             Focus Mode
 │                             ↓
 ↓                         Fullscreen
External Website              ↓
                          25-Min Timer
                              ↓
                         Session Complete
```

---

## 18. Project Structure

The current implementation is contained in a single HTML file.

```text
University-Academic-Portal/
│
└── index.html
    ├── HTML Structure
    ├── CSS Styling
    └── JavaScript Logic
```

### HTML

Responsible for the page structure and interface components.

### CSS

Responsible for the visual design, layouts, animations, responsiveness, and overlays.

### JavaScript

Responsible for dynamic behavior, redirects, search, fullscreen functionality, keyboard controls, and the Pomodoro timer.

---

## 19. Advantages

* Simple to run because it does not require a backend.
* No database setup is required.
* Demonstrates multiple frontend technologies.
* Contains both visual and functional components.
* Responsive across different screen sizes.
* Demonstrates browser APIs.
* Includes event-driven JavaScript.
* Combines practical UI development with humor.

---

## 20. Limitations

The project is primarily a frontend demonstration.

Current limitations include:

* No real authentication system.
* No backend server.
* No real student database.
* Academic statistics are static.
* Assignment information is static.
* Notifications are static.
* External services are opened instead of being integrated directly.
* Focus checklist state is not permanently saved.
* Timer state is lost when the page is refreshed.

---

## 21. Future Improvements

Possible future improvements include:

* Add a backend using Node.js, Flask, or Django.
* Add student login and authentication.
* Store student information in a database.
* Make attendance and academic scores dynamic.
* Add real assignment management.
* Add persistent notifications.
* Add user-specific dashboards.
* Save checklist progress using LocalStorage or a database.
* Allow customizable Pomodoro durations.
* Add short and long break modes.
* Add sound notifications when the timer ends.
* Add dark mode.
* Add real university API integrations.

---

## 22. Conclusion

The **University Academic Services Portal** demonstrates how HTML, CSS, and JavaScript can be combined to create a convincing interactive web application.

While the interface is designed to resemble a serious university academic portal, the project intentionally introduces humorous interactions through its service redirects. At the same time, the **Let's Chill** feature provides a genuinely functional focus environment with fullscreen control, a 25-minute Pomodoro timer, a checklist, interruption detection, and session completion handling.

Overall, the project combines **frontend development, JavaScript event handling, browser APIs, responsive UI design, and creative user interaction** into a single application.


# Screenshots 
<img width="1600" height="870" alt="WhatsApp Image 2026-09-12 at 3 16 48 AM" src="https://github.com/user-attachments/assets/ba419945-9499-4fe4-8ecb-8aea58259fe2" />

*Front page of our application

<img width="1600" height="875" alt="WhatsApp Image 2026-09-12 at 3 16 59 AM" src="https://github.com/user-attachments/assets/288c3b95-161d-4b23-9a00-50e58666d426" />

Page of our application accessing the lets chill button

<img width="1600" height="999" alt="image" src="https://github.com/user-attachments/assets/816cc3b5-d894-4678-9f96-ac5ad8020643" />

The Prank

# Diagrams
<img width="1024" height="1536" alt="WhatsApp Image 2026-09-12 at 3 30 17 AM" src="https://github.com/user-attachments/assets/1ea03f0b-4019-42a3-a799-94bad21774c2" />

Flowchart showing the working of our application

### Project Demo
# Video
https://drive.google.com/drive/folders/1ZFjlUiieiWc1lbThgQc-AWUdHG7QPwRZ?usp=drive_link
The video explains the working of the application or the website


## Team Contributions
Akshay J Nair: Designed and developed the university portal interface, dashboard layout, service cards, prank redirects, and overall project concept.
Adithya P: Assisted with HTML functionality, Focus Mode, timer implementation, testing, and project presentation.

---
Made with ❤️ at TinkerHub Useless Projects 

![Static Badge](https://img.shields.io/badge/TinkerHub-24?color=%23000000&link=https%3A%2F%2Fwww.tinkerhub.org%2F)
![Static Badge](https://img.shields.io/badge/UselessProjects--26-26?link=https%3A%2F%2Ftinkerhub.org%2Fevents%2F1M8ORET9A1%2Fuseless-projects-3.0)



