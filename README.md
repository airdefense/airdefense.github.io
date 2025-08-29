# AirDefense: Interactive Airspace Analysis Map

An interactive, browser-based mapping tool for visualizing and analyzing airspace activity. Add, move, and track various target types, analyze areas of interest, and save your scenarios as high-resolution images. This is a self-contained, single-file HTML application with no server-side dependencies.

<img width="1616" height="958" alt="Screenshot 2025-08-29 at 18 34 37" src="https://github.com/user-attachments/assets/bc5fb4f5-ce1f-4065-885c-78183ca5f7ff" />

## Features

-   **Interactive Map**: A dynamic map interface built on Leaflet.js with a dark-themed base layer.
-   **Add & Track Targets**:
    -   Place five distinct types of targets: Drone, Rocket, Ballistics, Aeroballistics, and Other.
    -   Click to place a target and drag the mouse to set its initial trajectory.
    -   Click and drag any target to move it; the path of movement is automatically traced with a gradient polyline, showing the direction of travel.
-   **Analyze Areas**:
    -   Draw a circle on the map to get a real-time count of all targets within that specific zone.
    -   The statistics panel updates instantly to reflect the contents of the analyzed area.
-   **Dynamic Statistics**: The top header provides an at-a-glance summary of all active targets on the map, categorized by type.
-   **History Controls**:
    -   **Undo/Redo**: Step backward or forward through your actions, including adding, moving, and deleting targets.
    -   **Clear All**: Instantly remove all targets and analysis circles from the map.
-   **Data Persistence**: Your session, including target positions, map view, and title, is automatically saved to your browser's local storage.
-   **Save as Image**: Export the current map view, including all targets and trails, as a high-quality PNG image for reports or briefings.
-   **Responsive UI**: The user interface is designed to be functional on both desktop and mobile devices.

<img width="1616" height="958" alt="Screenshot 2025-08-29 at 18 35 48" src="https://github.com/user-attachments/assets/636dd104-3096-49d9-b3e4-c785472a4a6a" />

## How to Use

1.  **Open the `index.html` file or [airdefense.github.io](airdefense.github.io)**: Since this is a standalone application, you can open it directly in any modern web browser.
2.  **Add a Target**:
    -   Select a target type (e.g., "Drone," "Rocket") from the "Tools" panel on the right.
    -   Click once on the map to set the target's starting point.
    -   Move your mouse to aim the target in the desired direction.
    -   Click a second time to confirm the placement.
3.  **Move a Target**: Click and drag any existing target. A trail will be drawn to show its path.
4.  **Delete a Target**:
    -   Click the "Delete Target" button in the Tools panel.
    -   Click on any target to mark it for deletion (it will become faded).
    -   Click it again to confirm the deletion.
5.  **Analyze an Area**:
    -   Click the "Analyze Area" button.
    -   Click and drag on the map to draw a circle.
    -   The stats in the top header will now reflect only the targets within that circle.
6.  **Save an Image**: Click the "Save as Image" button to download a PNG of the current map view.

<img width="3008" height="1518" alt="airdefense____2025-08-29" src="https://github.com/user-attachments/assets/ee07caf4-f6df-45b8-b5d8-c0d6c761297b" />

## Technologies Used

*   **HTML5 & CSS3**: For the structure and styling of the application.
*   **Vanilla JavaScript**: For all the application logic and interactivity.
*   **Leaflet.js**: A leading open-source JavaScript library for mobile-friendly interactive maps.
*   **Leaflet.draw**: A plugin for Leaflet that enables drawing and editing of shapes on the map.
*   **html2canvas**: A JavaScript library to capture screenshots of web pages or parts of it.
*   **L.RotatedMarker**: A Leaflet plugin to allow for marker rotation.
