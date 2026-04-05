# Spotify-Bot
Spotify OAuth Bot built using Python and Flask that implements OAuth 2.0 Authorization Code Flow, enabling secure user authentication and real-time access to Spotify data like profiles, playlists, and search functionality.

---

# 🎧 Spotify OAuth Bot

### ⚡ Secure Music Data Access with OAuth 2.0

<p align="center">
  <img src="https://readme-typing-svg.herokuapp.com?size=28&duration=2500&color=1DB954&center=true&vCenter=true&width=700&lines=Spotify+OAuth+Bot+🎧;Python+Flask+Backend+🐍;Secure+Authentication+🔐;Real-Time+Spotify+Integration" />
</p>

<p align="center">
  <img src="https://img.shields.io/badge/Python-3.10+-blue?style=for-the-badge&logo=python"/>
  <img src="https://img.shields.io/badge/Flask-Web%20Framework-black?style=for-the-badge&logo=flask"/>
  <img src="https://img.shields.io/badge/Spotify-API-1DB954?style=for-the-badge&logo=spotify"/>
  <img src="https://img.shields.io/badge/Auth-OAuth%202.0-green?style=for-the-badge"/>
</p>

---

## 🧠 Project Overview

This project demonstrates a **production-style implementation of OAuth 2.0 Authorization Code Flow** using Spotify.

It allows users to:

* Authenticate securely via Spotify
* Access personal data (profile, playlists)
* Interact with Spotify APIs in real-time

💡 Built with scalability and clean architecture in mind.

---

## 🏗️ Architecture

```id="qk9jgm"
Client → Spotify Auth Server → Callback → Flask Backend → Spotify API
```

* OAuth handled securely via backend
* Tokens managed with refresh mechanism
* REST APIs exposed for frontend integration

---

## ⚙️ Core Features

✨ **Authentication**

* OAuth 2.0 Authorization Code Flow
* Secure token exchange
* Refresh token lifecycle

🎯 **User Data**

* Fetch profile info
* Retrieve playlists
* Search music

⚡ **Backend Design**

* Modular architecture
* Service layer abstraction
* Clean route handling

---

## 🛠️ Tech Stack

| Layer   | Technology      |
| ------- | --------------- |
| Backend | Python (Flask)  |
| API     | Spotify Web API |
| Auth    | OAuth 2.0       |
| Config  | dotenv          |

---

## 📂 Project Structure

```id="8t1j6f"
spotify-oauth-bot/
│── app.py
│── auth.py
│── routes/
│   ├── user.py
│   ├── playlists.py
│── services/
│   ├── spotify_service.py
│── config/
│── .env
│── requirements.txt
```

---

## 🔄 OAuth Flow (Deep Dive)

1. User hits `/login`
2. Redirect → Spotify Authorization Server
3. User grants permission
4. Redirect back with `authorization_code`
5. Backend exchanges code → `access_token` + `refresh_token`
6. Secure API calls made

---

## 🚀 Getting Started

```bash id="0v7o1o"
git clone https://github.com/your-username/spotify-oauth-bot-python.git
cd spotify-oauth-bot-python
python -m venv venv
venv\Scripts\activate
pip install -r requirements.txt
python app.py
```

---

## 🔐 Environment Variables

```env id="d4h9l1"
CLIENT_ID=your_client_id
CLIENT_SECRET=your_client_secret
REDIRECT_URI=http://localhost:5000/callback
SECRET_KEY=your_secret_key
```

---

## 📌 API Endpoints

| Endpoint     | Description             |
| ------------ | ----------------------- |
| `/login`     | Start OAuth flow        |
| `/callback`  | Handle Spotify redirect |
| `/profile`   | Get user info           |
| `/playlists` | Fetch playlists         |
| `/search`    | Search tracks           |

---

## 📈 Why This Project Matters

✔ Demonstrates **real-world authentication system**
✔ Shows **API integration skills**
✔ Follows **clean backend architecture**
✔ Interview-ready explanation included

---

## 🧪 Future Enhancements

* 🎨 React Frontend Dashboard
* 🧠 AI-based music recommendations
* ☁️ Cloud deployment (AWS / Render)
* 📊 Analytics dashboard

---

## 🤝 Contribution

Open to improvements and feature suggestions!

---

## 📄 License

MIT License

---

## 👨‍💻 Author

**Ikchhita Bhatnagar**

💼 Aspiring Software Engineer


