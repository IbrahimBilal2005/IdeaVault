# IdeaVault

Flutter + FastAPI project.

---

## 🔧 Backend (FastAPI)

### 1. Setup
```bash
cd backend
python -m venv venv
venv\Scripts\activate  # On Windows
pip install -r requirements.txt
```

### 2. Run server
```bash
uvicorn main:app --reload
```

- Opens at: `http://localhost:8000`
- API docs: `http://localhost:8000/docs`

---

## 📱 Frontend (Flutter)

first install flutter: https://docs.flutter.dev/get-started/install
### 1. Setup
```bash
cd frontend
flutter pub get
```

### 2. Run the app
```bash
flutter run
```

---

## 🔌 API URL (in Flutter)

In `lib/config/api_config.dart`:

- Use this for Android emulator:
  ```dart
  static const String baseUrl = 'http://10.0.2.2:8000';
  ```

- Use this for physical device (update IP):
  ```dart
  static const String baseUrl = 'http://192.168.x.x:8000';
  ```


