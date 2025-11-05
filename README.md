# 📖 Local Animal Repository Generator

A Python application that reads structured animal data from a local JSON file, allowing the user to filter by skin type, and then generates a corresponding static HTML web page for display.

## ✨ Features

* **💾 Local Data Processing:** Reads taxonomy and characteristics directly from the required `data/animals_data.json` file.
* **🌐 Static Web Generation:** Creates a styled, ready-to-view HTML page (`web/animals.html`) to display the filtered animal data.
* **🎚️ Interactive Filtering:** Prompts the user to select a **skin type** (e.g., *Fur*, *Scales*) to filter the animals shown on the final web page.

---

## ⚙️ Setup & Execution

### 📋 Prerequisites

1.  **Python:** Ensure Python is installed on your system.
2.  **Data File:** Ensure the project includes the necessary `data/animals_data.json` file containing the animal records.

### ▶️ Run the Application

Navigate to the root directory in your terminal and execute the main script:

```bash
python animals_web_generator.py
````

### 🚶 Execution Flow

1.  **Filter Menu:** The program will greet you and present a numbered menu of unique skin types available in the data (e.g., `1. Fur`, `2. Scales`).
2.  **Input Selection:**
      * **Filter:** Enter the corresponding number (e.g., `1`) to display only animals matching that skin type.
      * **All Animals:** Leave the input **empty** and press **Enter**.
      * **Exit:** Select the **Exit** option (e.g., `4. Exit program`) to terminate.
3.  **View Output:** Upon successful execution, open the generated file **`web/animals.html`** in your web browser to view your new animal repository\!

-----

## 🏗️ Project Structure (For Developers)

The core logic is modularized for clarity:

| Module / Directory | Responsibility |
| :--- | :--- |
| `animals_web_generator.py` | Main entry point; handles user input (filter selection) and orchestrates web page generation. |
| `data/` | Contains the source data (`animals_data.json`) and the data loading logic (`json_manager.py`). |
| `web/` | HTML templating (`animals_template.html`), final output (`animals.html`), and HTML generation logic (`html_manager.py`). |
