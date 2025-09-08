# Daily Bites

Daily Bites is a full-stack web application for tracking daily meals, calories, and nutrition. It features a Django REST API backend and a modern React frontend.

## Features

- User authentication and profile management
- Upload and manage profile images
- Log daily meals and track nutritional intake
- View daily calorie and macronutrient goals
- Responsive and user-friendly interface

## Tech Stack

- **Frontend:** React, Tailwind CSS, Vite
- **Backend:** Django, Django REST Framework, Knox authentication
- **Database:** SQLite (default, can be changed)
- **Other:** CORS, dotenv for environment management

## Project Structure

```
django-backend/
    food_diary_app/
        accounts/      # User accounts and authentication
        meal/          # Meal and nutrition tracking
    manage.py
    requirements.txt

react-frontend/
    src/
        components/    # Reusable UI components
        pages/         # Main application pages
        assets/        # Images and static assets
    package.json
    tailwind.config.cjs
```

## Getting Started

### Backend Setup

1. **Install dependencies:**
    ```sh
    cd django-backend
    pip install -r requirements.txt
    ```

2. **Set environment variables:**
    - Create a `.env` file in `django-backend/food_diary_app/` with your `SECRET_KEY` and other settings.

3. **Run migrations:**
    ```sh
    python manage.py migrate
    ```

4. **Start the server:**
    ```sh
    python manage.py runserver
    ```

### Frontend Setup

1. **Install dependencies:**
    ```sh
    cd react-frontend
    npm install
    ```

2. **Start the development server:**
    ```sh
    npm run dev
    ```

3. **Access the app:**
    - Frontend: [http://localhost:5173](http://localhost:5173)
    - Backend API: [http://localhost:8000](http://localhost:8000)

## Environment Variables

- **Backend:**  
  See `django-backend/food_diary_app/settings.py` for required environment variables.
- **Frontend:**  
  Configure API endpoints as needed in `src/customAxios.js`.

## License

This project is licensed under the MIT License.

---

**Daily Bites** – Track your nutrition, reach