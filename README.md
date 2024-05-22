# Detection-of-Overloading-in-Public-Transport
1. Project Planning and Requirement Analysis
- Define Objectives: Establish the goals of the project, such as detecting and counting people, tracking bus location, and providing alerts for overcrowding.
- Gather Requirements: Identify the hardware (camera, GPS module) and software (MobilenetSSD, Supabase, dashboard development tools) needed.
- Feasibility Study: Assess the technical and economic feasibility of the project.
2. System Design
- Architecture Design :  Design the overall system architecture, including data flow from the camera to the dashboard.
- Component Selection: Choose appropriate components:
 - Camera : For capturing real-time video footage.
  - GPS Module: For tracking the bus location.
  - Server: For processing and storing data.
  - Database: Supabase for storing data.
  - Dashboard: For live monitoring and alerts.
3. MobilenetSSD Implementation for People Detection
- Model Setup: Download and set up the MobilenetSSD Caffe model.
- Video Feed Integration: Integrate the camera feed with the MobilenetSSD model for real-time detection.
- Code Implementation: Write the code to detect people in the video stream.
- Validation: Test the model to ensure accurate detection of people.
 4. Counting Mechanism
- Line of Intersection: Define a line of intersection in the video feed for counting people.
- Counting Logic : Implement the logic to:
  - Count as enter when a person crosses the line from outside.
  - Count as exit:  when a person crosses the line from inside.
  - Increment or decrement the count accordingly.
- Testing: Validate the counting mechanism with various scenarios.
5. Location Tracking
- GPS Integration: Integrate the GPS module to fetch the bus location.
- Data Synchronization: Ensure real-time synchronization of the location data with the system.
 6. Data Storage and Management with Supabase
- Database Design: Design the database schema on Supabase to store:
  - People count data.
  - Bus location data.
  - Timestamps.
- API Integration: Use Supabase APIs to:
  - Insert and retrieve data.
  - Maintain the database connection.
7. Dashboard Development
- Interface Design: Design the user interface for the dashboard to display:
  - Real-time people count.
  - Live bus location on a map.
  - Alerts for overcrowding.
- Frontend Development: Develop the frontend using suitable frameworks (e.g., React, Angular).
- Backend Development: Develop the backend to handle data from the detection system and GPS module.
8. Overcrowding Alert System
- Threshold Setting: Define a threshold for overcrowding.
- Alert Mechanism: Implement the logic to:
  - Monitor the people count.
  - Trigger an alert if the count exceeds the threshold.
- Notification System: Develop a notification system to display alerts on the dashboard.
 9. Integration and Testing
- System Integration: Integrate all components into a cohesive system.
- End-to-End Testing: Conduct comprehensive testing to ensure:
  - Accurate people detection and counting.
  - Correct GPS location tracking.
  - Real-time data updates on the dashboard.
  - Proper functioning of the alert system.
- Debugging: Identify and fix any issues or bugs.
10. Deployment and Final Review
- Deployment: Deploy the system on the intended hardware setup (e.g., bus).
- User Training: Provide training for end-users on how to use the dashboard and interpret alerts.
- Documentation: Prepare detailed documentation of the project, including:
  - System architecture and design.
  - Installation and setup instructions.
  - User manual.
- Final Presentation : Present the project to stakeholders, demonstrating the system's functionality and benefits.
