### Kanban Board Application
## Table of Contents
#Overview
#Features
#Design
#Technologies-Used
#Installation
#Usage
#Project-Structure
#API-Integration
#State-Management
#Styling
#Persisting-State
#Evaluation-Criteria
#Assets
#Notes
#Overview
This project is an interactive Kanban Board application built using React JS. The application fetches ticket data from a provided API and allows users to group and sort tickets based on different criteria. The user interface is designed to be responsive and visually appealing, closely following the provided design specifications.

#Features
Dynamic Grouping: Users can group tickets by Status, User, or Priority.
Sorting Options: Tickets can be sorted by Priority (descending) or Title (ascending).
Responsive Design: The application is fully responsive and maintains visual integrity across various devices.
State Persistence: User preferences for grouping and sorting are saved and persist across page reloads.
Interactive UI: Smooth and intuitive user interactions aligning with the provided design mockups.
#Design
The application's design mirrors the provided screenshots, ensuring consistency in layout, card design, and overall aesthetics. The Kanban board adjusts dynamically based on user selections for grouping and sorting, providing a seamless user experience.

Display States
Grouped by User:

Grouped by Priority:

Card View:

#Technologies-Used
React JS: Frontend library for building the user interface.
Pure CSS: Custom styling without the use of CSS libraries.
Local Storage: For persisting user state across sessions.
Fetch API: To retrieve data from the provided backend API.
#Installation
Prerequisites
Node.js (v14 or above)
npm or yarn
Steps
Clone the Repository

bash
Copy code
git clone https://github.com/your-username/kanban-board.git
cd kanban-board
Install Dependencies

Using npm:

bash
Copy code
npm install
Or using yarn:

bash
Copy code
yarn install
Start the Development Server

Using npm:

bash
Copy code
npm start
Or using yarn:

bash
Copy code
yarn start
Access the Application

Open your browser and navigate to http://localhost:3000 to view the application.

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
#Project-Structure
csharp
Copy code
kanban-board/
├── public/
│   ├── index.html
│   └── assets/
├── src/
│   ├── components/
│   │   ├── KanbanBoard.jsx
│   │   ├── TicketCard.jsx
│   │   ├── GroupingOptions.jsx
│   │   └── SortingOptions.jsx
│   ├── services/
│   │   └── api.js
│   ├── styles/
│   │   └── styles.css
│   ├── App.jsx
│   ├── index.js
│   └── utils/
│       └── helpers.js
├── .gitignore
├── package.json
├── README.md
└── yarn.lock / package-lock.json
#API-Integration
The application interacts with the provided API endpoint to fetch ticket data.

API Endpoint: https://api.quicksell.co/v1/internal/frontend-assignment
Fetching Data
Use the fetch API to retrieve data.
Handle loading states and potential errors during data fetching.
Data Structure
Tickets received from the API include:

id: Unique identifier
title: Title of the ticket
description: Detailed description
status: Current status (e.g., Open, In Progress, Closed)
priority: Priority level (0-4)
assignedUser: User assigned to the ticket
#State-Management
Local Component State: Manage component-specific states using React’s useState.
Global State: Use React's useContext or useReducer if necessary for managing global states.
Persisting State: Use localStorage to save and retrieve user preferences for grouping and sorting.
#Styling
Pure CSS: All styles are written in standard CSS without any libraries.
Modular CSS: Organize styles into modular and reusable classes.
Responsive Design: Ensure the application is responsive across different screen sizes using media queries and flexible layouts.
#Persisting-State
To ensure user preferences persist across page reloads:

Saving State:

On grouping or sorting option change, save the selected options to localStorage.
Retrieving State:

On application load, check localStorage for existing preferences.
Apply the saved preferences to initialize the application's state.
#Evaluation-Criteria
Your submission will be evaluated based on the following criteria:

Functionality:

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
#Assets
Design Assets: Download Assets
#Notes
CSS Libraries: Do not use any CSS libraries such as Bootstrap, Tailwind, Material UI, Chakra, etc. All styling must be done using pure CSS or Styled JSX.

Frameworks: Do not use frameworks like Next.js. The application should be built using pure React JS.

API Priority Levels:

The API provides priority levels as integers. Map them as follows:

4: Urgent
3: High
2: Medium
1: Low
0: No priority
