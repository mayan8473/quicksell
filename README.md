# Kanban Board Application
## Table of Contents
Overview
Features
Design
Technologies-Used
Installation
Usage
Project-Structure
API-Integration
State-Management
Styling
Persisting-State
Evaluation-Criteria
Assets
Notes
# Overview
This project is an interactive Kanban Board application built using React JS. The application fetches ticket data from a provided API and allows users to group and sort tickets based on different criteria. The user interface is designed to be responsive and visually appealing, closely following the provided design specifications.

# Features
Dynamic Grouping: Users can group tickets by Status, User, or Priority.
Sorting Options: Tickets can be sorted by Priority (descending) or Title (ascending).
Responsive Design: The application is fully responsive and maintains visual integrity across various devices.
State Persistence: User preferences for grouping and sorting are saved and persist across page reloads.
Interactive UI: Smooth and intuitive user interactions aligning with the provided design mockups.
# Design
The application's design mirrors the provided screenshots, ensuring consistency in layout, card design, and overall aesthetics. The Kanban board adjusts dynamically based on user selections for grouping and sorting, providing a seamless user experience.

# Display States
Grouped by User,
Grouped by Priority,
Card View

# Technologies-Used
React JS: Frontend library for building the user interface.
Pure CSS: Custom styling without the use of CSS libraries.
Local Storage: For persisting user state across sessions.
Fetch API: To retrieve data from the provided backend API.
# Installation
Prerequisites
Node.js (v14 or above)
npm or yarn
Install Dependencies
Using npm:
#Usage
Grouping Tickets:

Click on the "Display" button.
Select a grouping option: By Status, By User, or By Priority.
The Kanban board will adjust to reflect the selected grouping.
Sorting Tickets:

Choose a sorting option: Priority (descending) or Title (ascending).
Tickets within each group will reorder based on the selected sorting criteria.
Persisted State:

The application saves your grouping and sorting preferences.
Reloading the page retains your last selected view.
# Functionality:

Effective data fetching from the provided API.
Accurate grouping and sorting of tickets based on user selections.
Persistence of user preferences across sessions.
Visual Design:

UI matches the provided design screenshots.
Consistent layout, card design, and overall aesthetics.
Business Logic Optimization:

Efficient data handling and state management.
Minimization of unnecessary re-renders and performance optimizations.
Component Structuring:

Properly structured components promoting reusability and maintainability.
Clear separation of concerns and modular architecture.
# Assets
Design Assets: Download Assets
# Notes
CSS Libraries: Do not use any CSS libraries such as Bootstrap, Tailwind, Material UI, Chakra, etc. All styling must be done using pure CSS or Styled JSX.

Frameworks: Do not use frameworks like Next.js. The application should be built using pure React JS.

