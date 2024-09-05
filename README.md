
# SwapShop Project

This project is a web-based application built using the Flask framework in Python. It appears to have a database and various charts or visualizations. Below are the instructions on how to set up and use the project.

## Prerequisites

Before running this project, ensure you have the following installed:

- **Python** (preferably 3.6+)
- **pip** (Python package manager)
- **Flask** (web framework)
- **SQLite** (database used in this project)
- **A virtual environment** tool like `venv` or `virtualenv` (optional but recommended)

## Setup Instructions

### 1. Clone or Download the Project
Make sure the project folder is downloaded or cloned into your working directory.

### 2. Create a Virtual Environment (Optional)

It's a good practice to create a virtual environment to manage your project dependencies. Run the following commands:

```bash
# On macOS and Linux
python3 -m venv venv

# On Windows
python -m venv venv
```

Activate the virtual environment:

```bash
# On macOS and Linux
source venv/bin/activate

# On Windows
venv\Scripts\activate
```

### 3. Install Required Python Packages

In the terminal, navigate to the project folder where `main.py` is located and install Flask and other dependencies by running the following command:

```bash
pip install Flask
```
If the ask more dependecies install all dependencies using pip


### 4. Run the Flask Application

To start the Flask application, navigate to the project directory and run the `main.py` file:

```bash
# On macOS and Linux
export FLASK_APP=main.py

# On Windows
set FLASK_APP=main.py

# Run the Flask app
flask run
```

This will start a local server. You should see output similar to:

```
* Running on http://127.0.0.1:5000/ (Press CTRL+C to quit)
```

### 5. Access the Application

Once the application is running, open your browser and navigate to:

```
http://127.0.0.1:5000
```

### 6. Directory Structure

Here’s a detailed view of the folder structure of the project:

```
swapshop/
│
├── __pycache__/                
├── baryearly.py                # Python file for bar chart generation
├── main.py                     # Main entry point of the application
├── mybaryear.py                # Python file for handling bar charts per year
├── mychart.py                  # Python file for general chart generation
├── mypie.py                    # Python file for generating pie charts
├── peryear.py                  # Data processing for yearly comparisons
├── pieyearly.py                # Python file for yearly pie chart generation
├── swapshop.db                 # SQLite database file
│
├── static/                     # Static files (e.g., CSS, JavaScript, images)
│   ├── css/                    # Custom CSS for styling
│   ├── js/                     # JavaScript files
│   └── img/                    # Images used in the application
│
├── templates/                  # HTML templates for the frontend
│   ├── base.html               # Base HTML template
│   ├── chart.html              # Template for displaying charts
│   ├── index.html              # Home page of the application
│   └── piechart.html           # Template for displaying pie charts
│
└── README.md                   # Project documentation (this file)
```

### 7. Editing the Templates

The HTML files inside the `templates` directory are responsible for the frontend of the application. You can modify these templates to change the design and layout of the app.

### 8. Database Setup

This project uses an SQLite database (`swapshop.db`). If necessary, you can inspect or modify the database using any SQLite management tool.

