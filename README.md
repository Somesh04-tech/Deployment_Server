📦 Django REST API – Item Management with HTML File Uploads
📖 Overview

This project is a Django REST Framework (DRF)–based API that allows users to create, read, update, and delete (CRUD) items, where each item can have an associated HTML file uploaded and stored on the server.

It can be used as a content management system (CMS), deployment manager, or HTML-based page storage service, enabling structured management of uploaded HTML files through RESTful APIs.

🚀 Features

🔄 Full CRUD operations using REST APIs

📄 Upload and manage HTML files per item

🌐 CORS-enabled for frontend integration

🗂️ Organized file storage (html/ directory)

🛠️ Built with Django + Django REST Framework

💾 Uses SQLite for lightweight storage

🔐 Ready for extension with authentication & permissions

🧱 Tech Stack
Technology	Description
Django	Backend web framework
Django REST Framework	API development
SQLite	Database
django-cors-headers	Cross-Origin Resource Sharing
Python	Programming language

📂 Project Structure (Simplified)
project_root/
│
├── items/
│   ├── models.py
│   ├── serializers.py
│   ├── views.py
│   ├── urls.py
│
├── html/                  # Uploaded HTML files stored here
│
├── project/
│   ├── settings.py
│   ├── urls.py
│
├── manage.py
└── README.md
🧩 Data Model

Each Item contains:

name – Item title

description – Brief description

html_file – Uploaded .html file (optional)

🔌 API Endpoints
Method	Endpoint	Description
GET	/api/items/	List all items
POST	/api/items/	Create a new item
GET	/api/items/<id>/	Retrieve a specific item
PUT	/api/items/<id>/	Update an item
DELETE	/api/items/<id>/	Delete an item

📌 File uploads are handled using multipart/form-data
🔮 Future Improvements

🔐 Authentication & authorization (JWT / Token)

📁 HTML file preview in browser

🧪 Unit & API testing

📦 PostgreSQL support

🚀 Docker deployment