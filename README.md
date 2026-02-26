# 📝 Student Form Full‑Stack Application

A simple full‑stack project that lets users create and view student records.  
The backend is built with **Django + Django REST Framework**, while the frontend is a **React** single‑page app.

---

## 📁 Project Structure

```
backend/           ← Django project
  ├─ backend/      ← core settings, URLs, WSGI/ASGI
  ├─ students/     ← app with models, serializers, views, tests
  ├─ db.sqlite3
  └─ manage.py

frontend/          ← React application
  ├─ public/
  └─ src/
      └─ components/StudentForm.js
```

---

## 🚀 Getting Started

### Backend

1. **Create & activate a virtual environment**  
   ```powershell
   python -m venv venv
   .\venv\Scripts\Activate
   ```

2. **Install dependencies**  
   ```powershell
   pip install -r backend/requirements.txt
   ```

3. **Apply migrations**  
   ```powershell
   cd backend
   python manage.py migrate
   ```

4. **Run the development server**  
   ```powershell
   python manage.py runserver
   ```

   API will be available at `http://localhost:8000/`.

### Frontend

1. **Install packages**  
   ```powershell
   cd frontend
   npm install
   ```

2. **Start the React app**  
   ```powershell
   npm start
   ```

   The UI opens at `http://localhost:3000/` and interacts with the Django API.

---

## 🛠 Features

- Add new students with name, age, department, marks, etc.
- View a list of students (API endpoint + simple form component).
- Django REST‑powered backend with serializers and viewsets.
- React form component (`StudentForm.js`) for frontend input.

---

## 🧪 Testing

- Backend tests located in `backend/students/tests.py`.  
  Run them with `python manage.py test`.

---

## 🔧 Configuration

- Django settings in `backend/backend/settings.py`.
- API routes defined in `backend/students/urls.py` and `backend/backend/urls.py`.
- React components in `frontend/src/components`.

---

## 📄 License

This project is open source. Feel free to fork and modify!

---

> 💡 **Tip:** You can extend the app by adding authentication, advanced validation, or deploying to Heroku/Vercel.

Happy coding! 🎉