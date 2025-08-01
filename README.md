# Wagtail Tutorial - First Site

This repository contains a Wagtail blog application following the official Wagtail tutorial.

## About
This project is a basic blog application built with Wagtail CMS, following the [Wagtail Tutorial](https://docs.wagtail.org/en/stable/getting_started/tutorial.html).

## Features
- A public site with a blog
- Wagtail admin interface for content management
- Blog posts with rich text content
- Blog index page showing published posts
- Basic blog post functionality

## Setup
1. Clone the repository: `git clone https://github.com/ntumngiar/wagtail-tutorial-1.git`
2. Navigate to the project: `cd wagtail-tutorial-1/mysite`
3. Create a virtual environment: `python -m venv env`
4. Activate the virtual environment:
   - Windows: `env\Scripts\activate`
   - Unix/MacOS: `source env/bin/activate`
5. Install dependencies: `pip install -r requirements.txt`
6. Run migrations: `python manage.py migrate`
7. Create a superuser: `python manage.py createsuperuser`
8. Run the development server: `python manage.py runserver`
9. Visit http://127.0.0.1:8000/ to see the site
10. Visit http://127.0.0.1:8000/admin/ to access the Wagtail admin interface

## Tutorial Progress
- ✅ Basic Wagtail installation
- ✅ Extended HomePage model with RichTextField
- ✅ Created blog app
- ✅ Created BlogIndexPage and BlogPage models
- ✅ Set up templates for blog pages
- ✅ Implemented get_context override for proper blog post ordering
- 🔄 Working on images, authors, and tags features

## Technology Stack
- Python 3.12
- Django 5.2
- Wagtail 7.0
- SQLite (development database)
