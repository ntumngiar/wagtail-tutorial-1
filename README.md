# Wagtail Tutorial - Complete Portfolio Site

This repository contains a complete Wagtail portfolio site following the official Wagtail tutorial with all advanced features implemented.

## About
This project is a comprehensive portfolio website built with Wagtail CMS, following the [Official Wagtail Tutorial](https://docs.wagtail.org/en/stable/tutorial/index.html). It demonstrates all major Wagtail features and best practices.

## Features
- **Homepage with Hero Section** - Dynamic hero image, text, and call-to-action
- **Portfolio Page with StreamField** - Flexible content blocks for showcasing projects
- **Contact Forms** - Dynamic form builder with email notifications
- **Blog System** - Full blog with posts, categories, and search
- **Site Navigation** - Dynamic menu system with page management
- **Search Functionality** - Full-text search with pagination
- **Footer Management** - Editable footer text and social media links
- **Responsive Design** - Mobile-friendly styling and accessibility features
- **Admin Interface** - Complete Wagtail CMS for content management

## Quick Start
1. Clone the repository: `git clone https://github.com/ntumngiar/wagtail-tutorial-1.git`
2. Navigate to the project: `cd wagtail-tutorial-1/mysite`
3. Create a virtual environment: `python -m venv env`
4. Activate the virtual environment:
   - **Windows PowerShell**: `& ".\env\Scripts\Activate.ps1"`
   - **Windows CMD**: `env\Scripts\activate`
   - **Unix/MacOS**: `source env/bin/activate`
5. Install dependencies: `pip install -r requirements.txt`
6. Run migrations: `python manage.py migrate`
7. Create a superuser: `python manage.py createsuperuser`
8. Run the development server: `python manage.py runserver`
9. Visit http://127.0.0.1:8000/ to see the site
10. Visit http://127.0.0.1:8000/admin/ to access the Wagtail admin interface

## Running the Application

### Start the Development Server
```bash
# Navigate to project directory
cd wagtail-tutorial-1/mysite

# Activate virtual environment (Windows PowerShell)
& ".\env\Scripts\Activate.ps1"

# Or for Windows CMD
env\Scripts\activate

# Or for Unix/MacOS
source env/bin/activate

# Start the server
python manage.py runserver
```

### Access the Application
- **Main Site**: http://127.0.0.1:8000/
- **Admin Interface**: http://127.0.0.1:8000/admin/
- **Search**: http://127.0.0.1:8000/search/


### Database and Media Files
Content created through Wagtail admin is stored in:
- **Database**: `db.sqlite3` (SQLite database file)
- **Media Files**: `media/` directory (uploaded images, documents)

## Version Control and Deployment

### Saving Your Changes
When you make changes through the Wagtail admin (adding pages, uploading images, etc.), you need to commit the database and media files:

```bash
# Add all changes including database and media files
git add .

# Commit with descriptive message
git commit -m "Add portfolio page, contact form, and hero images

# Push to repository
git push
```

### Important Files to Commit
- `db.sqlite3` - Contains all your content (pages, forms, settings)
- `media/` - Contains uploaded images and documents
- Any code changes you made to templates or models


## Technology Stack
- **Python 3.12**
- **Django 5.2**
- **Wagtail 7.0**
- **SQLite** (development database)
- **HTML5/CSS3** with responsive design
- **JavaScript** for enhanced interactivity



### Committing Changes
```bash
# For content changes made through admin
git add db.sqlite3 media/
git commit -m "Update site content and images"

# For code/template changes
git add templates/ static/ *.py
git commit -m "Update site design and functionality"

# For both content and code changes
git add .
git commit -m "Complete site update with new content and features"
```

### Reset Development Database
If you need to start fresh:
```bash
# Delete database and media files
rm db.sqlite3
rm -rf media/

# Recreate database
python manage.py migrate
python manage.py createsuperuser
```
