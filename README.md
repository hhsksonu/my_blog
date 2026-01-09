# Django Blog Website (HHSKSONU'S BLOG)

A fully functional personal blog application built with Django framework featuring a clean, modern interface for sharing thoughts on technology, travel, and more.

## Live Demo

**[Visit Live Site](https://hhsksonu.pythonanywhere.com/)**

## Features

- **Personal Blog Platform**: Share articles on technology, programming, travel, and lifestyle
- **Blog Post Management**: Create, read, update, and delete blog posts with rich content
- **Featured Images**: Each post includes eye-catching featured images
- **Read Later Functionality**: Save posts to read later with a dedicated stored posts section
- **Post Preview**: Browse all posts with titles, excerpts, and featured images
- **Responsive Design**: Mobile-friendly interface with modern, clean styling
- **Admin Panel**: Comprehensive Django admin dashboard for content management
- **Media Management**: Upload and manage post images efficiently
- **Author Profile**: Personalized author section showcasing blog identity

## 📸 Sample Posts

The blog features diverse content including:
- Technology and programming tutorials (Python Programming)
- Travel and adventure stories (Mountain Hiking)
- Cultural insights (India Is Great)
- And more!

## 🛠️ Technologies Used

- **Backend**: Django (Python web framework)
- **Database**: SQLite (Development) / PostgreSQL (Production ready)
- **Frontend**: HTML, CSS, JavaScript
- **Deployment**: PythonAnywhere
- **Media Storage**: Django Media Files

## Project Structure

```
Blog-website-Django/
├── blog/                 # Main blog application
│   ├── models.py        # Post, Comment, Author models
│   ├── views.py         # View logic for blog pages
│   ├── urls.py          # URL routing for blog
│   └── admin.py         # Admin panel configuration
├── my_blog/             # Project settings and configurations
│   ├── settings.py      # Django settings
│   ├── urls.py          # Main URL configuration
│   └── wsgi.py          # WSGI configuration
├── static/              # Static files (CSS, JS, images)
│   └── blog/
│       └── images/      # Static images (author photo, etc.)
├── templates/           # HTML templates
│   ├── base.html        # Base template
│   ├── index.html       # Home page
│   ├── all-posts.html   # All posts listing
│   └── post-detail.html # Individual post view
├── uploads/posts/       # Uploaded post images
├── media/posts/         # Media files
├── db.sqlite3          # SQLite database
├── manage.py           # Django management script
└── requirements.txt    # Project dependencies
```

## Installation

### Prerequisites

- Python 3.8 or higher
- pip (Python package manager)
- virtualenv (recommended)
- Git

### Setup Instructions

1. **Clone the repository**
   ```bash
   git clone https://github.com/hhsksonu/Blog-website-Django.git
   cd Blog-website-Django
   ```

2. **Create a virtual environment**
   ```bash
   python -m venv venv
   ```

3. **Activate the virtual environment**
   - On Windows:
     ```bash
     venv\Scripts\activate
     ```
   - On macOS/Linux:
     ```bash
     source venv/bin/activate
     ```

4. **Install dependencies**
   ```bash
   pip install -r requirements.txt
   ```

5. **Configure settings**
   - Update `my_blog/settings.py` if needed
   - Set `DEBUG = True` for local development
   - Configure `ALLOWED_HOSTS` as needed

6. **Run migrations**
   ```bash
   python manage.py makemigrations
   python manage.py migrate
   ```

7. **Create a superuser** (for admin access)
   ```bash
   python manage.py createsuperuser
   ```
   Follow the prompts to create your admin account.

8. **Collect static files** (if needed)
   ```bash
   python manage.py collectstatic
   ```

9. **Run the development server**
   ```bash
   python manage.py runserver
   ```

10. **Access the application**
    - Main site: `http://localhost:8000/`
    - Admin panel: `http://localhost:8000/admin/`

## Usage

### Creating Blog Posts

1. Log in to the admin panel at `/admin`
2. Navigate to "Posts" section
3. Click "Add Post"
4. Fill in:
   - Title
   - Slug (URL-friendly version)
   - Excerpt (brief description)
   - Content (full article)
   - Featured image
5. Save and publish

### Managing Stored Posts

- Users can save posts to read later
- Access saved posts via the "Stored Post" link in navigation
- Easy bookmark functionality for content management

### Viewing Content

- **Home Page**: Features latest thoughts and author introduction
- **All Posts**: Browse complete collection of blog posts
- **Individual Posts**: Click any post to read full content

## Customization

### Styling
- CSS files are located in `static/blog/css/`
- Modify templates in `templates/` directory
- Update author image in `static/blog/images/`

### Content
- Author bio can be edited in the home page template
- Site title and metadata in `settings.py`
- Navigation links in base template

## Deployment

This project is deployed on PythonAnywhere. For your own deployment:

### PythonAnywhere Deployment

1. Create a PythonAnywhere account
2. Upload your code via Git or manual upload
3. Set up a virtual environment
4. Configure WSGI file
5. Set static files mapping
6. Update `ALLOWED_HOSTS` in settings
7. Run migrations on the server

### Other Deployment Options

- **Heroku**: Use Gunicorn and configure Procfile
- **DigitalOcean**: Deploy on a droplet with Nginx
- **AWS**: Use Elastic Beanstalk or EC2
- **Render**: Simple deployment with automatic builds

## Contributing

Contributions are welcome! Here's how you can help:

1. Fork the repository
2. Create a feature branch (`git checkout -b feature/AmazingFeature`)
3. Make your changes
4. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
5. Push to the branch (`git push origin feature/AmazingFeature`)
6. Open a Pull Request

## License

This project is open source and available for educational purposes.

## Author

**HHSKSONU**
- Blog: [hhsksonu.pythonanywhere.com](https://hhsksonu.pythonanywhere.com/)
- GitHub: [@hhsksonu](https://github.com/hhsksonu)

## Acknowledgments

- Django framework for robust backend functionality
- PythonAnywhere for reliable hosting
- Open source community for inspiration and resources

---

**Note**: This project serves as a portfolio piece and learning demonstration. For production use with sensitive data, implement additional security measures including environment variables for secret keys, HTTPS enforcement, and secure database configuration.
