# **FLASK WEB APPLICATION**

This is a simple Flask web application built with Python 3.11. It features a homepage and an API endpoint. Additionally, it includes Docker support for containerization.

### **Project Structure:**

------

```
my_flask_app/
│
├── static/
│└── styles.css
│
├── templates/
│├── index.html
│
├── app.py
├── requirements.txt
├── Dockerfile
└── README.md
```



- `app.py`: The main Flask application file containing routes and API endpoints.
- `static/css/styles.css`: The CSS stylesheet for styling the web pages.
- `templates/index.html`: The HTML template for the homepage.
- `templates/api_response.html`: The HTML template to display API responses.
- `requirements.txt`: Lists the dependencies for the Flask application.
- `Dockerfile`: Defines the container image for the Flask application.

------

### Setup and Installation

------

#### Prerequisites

- Python 3.11
- Docker (for containerization)

#### Installation

1. **Clone the repository**:

   ```
   git clone https://github.com/rajatchauhan-git/flask-app.git
   cd flask-app
   ```

   

2. **Create Dockerfile**
   
   

#### Docker Setup

1. **Build the Docker image**:

   ```
   docker build -t flask-app:v1 .
   ```

   

2. **Run the Docker container**:

   ```
   docker run --name flask -p 4000:4000 flask-app:v1
   ```

   

   Access the application at `http://localhost:4000/`.
   
   

### Usage

------

- **Homepage**: Displays a welcome message and basic information about the application.

- **API Endpoint**: Accessible at `/api` and returns a JSON response with sample data.
