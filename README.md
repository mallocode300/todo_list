# Todo List Application

A simple, modern todo list web application built with Flask. Features include:
- Add new tasks
- Mark tasks as complete/incomplete
- Delete tasks
- Export todo list to PDF
- Responsive design
- SQLite database for data persistence

## Local Development

1. Create a virtual environment:
```bash
python -m venv venv
source venv/bin/activate  # On Windows, use: venv\Scripts\activate
```

2. Install dependencies:
```bash
pip install -r requirements.txt
```

3. Run the application:
```bash
python app.py
```

4. Open your browser and navigate to `http://localhost:5000`

## GitHub Setup

1. Initialize a new Git repository:
```bash
git init
```

2. Add your files:
```bash
git add .
```

3. Make your first commit:
```bash
git commit -m "Initial commit"
```

4. Create a new repository on GitHub

5. Link your local repository to GitHub:
```bash
git remote add origin https://github.com/YOUR_USERNAME/todo_list.git
git branch -M main
git push -u origin main
```

## Deployment on Render.com

1. Create a new Web Service on Render.com
2. Connect your GitHub repository
3. Use the following settings:
   - Build Command: `pip install -r requirements.txt`
   - Start Command: `gunicorn app:app`
4. Add the following environment variables:
   - `PYTHON_VERSION`: `3.9.0`
   - `FLASK_ENV`: `production`

## Features

- Clean, modern UI using Bootstrap 5
- Responsive design that works on all devices
- Real-time task updates
- PDF export functionality
- SQLite database for data persistence
- Easy deployment to Render.com

## Technologies Used

- Flask
- SQLAlchemy
- Bootstrap 5
- ReportLab (for PDF generation)
- SQLite
- Gunicorn (for production deployment)

## Project Structure

```
todo_list/
├── app.py              # Main application file
├── requirements.txt    # Project dependencies
├── Procfile           # For Render deployment
├── runtime.txt        # Python version specification
├── templates/         # HTML templates
│   └── index.html     # Main template
└── instance/          # Database files (not in git)
    └── todo.db        # SQLite database
```

## Contributing

Feel free to fork this repository and submit pull requests. For major changes, please open an issue first to discuss what you would like to change.

## License

This project is open source and available under the MIT License. 