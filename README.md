# VehicleReID-App

<img width="3828" height="2071" alt="image" src="https://github.com/user-attachments/assets/f78e3545-6774-4c39-a0ed-295a64f841aa" />

# Vehicle Re-ID and Segmentation Query GUI

This application provides a graphical user interface (GUI) for vehicle re-identification (Re-ID) with an advanced segmentation-based search feature.

## Key Features

*   **Vehicle Detection**: Select an image, and the application uses a YOLO model to automatically detect all vehicles present.
*   **Interactive Query**: Simply click on any detected vehicle in the query image to select it for a search.
*   **Vehicle Re-Identification**: Once a vehicle is selected, the system extracts its unique features using a deep learning Re-ID model (trained on the VeRi-776 dataset) and searches a database for the most similar vehicles.
*   **Top-N Results**: The application displays the top matching vehicles from the database, ranked by similarity.
*   **Advanced Segmentation**:
    *   The selected vehicle can be segmented into its constituent parts (e.g., roof, windows, doors, face, rear).
    *   This is achieved using a DeepLabV3+ segmentation model (trained on the MVP-24 dataset).
*   **Segment-Based Search**:
    *   Users can select a specific segment of the query vehicle (e.g., just the "left-body" or "roof").
    *   The system can then perform a search to find vehicles in the database that have a similar-looking segment.
*   **Combined Scoring**: The search results can be refined by combining the similarity scores from both the whole vehicle and the selected segment. The user can adjust the weights given to each score to fine-tune the search.
*   **Modern and User-Friendly Interface**: The application is built with Tkinter and features a modern, intuitive layout with tooltips and interactive controls.

This tool is designed for detailed vehicle analysis, allowing for powerful searches that go beyond simple appearance matching by focusing on specific vehicle parts.

---

*The source code for this application will be made available soon.*
