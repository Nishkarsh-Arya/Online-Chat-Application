# 💬 Online Chat Application (PHP + MySQL)

This is a real-time chat application built using PHP, MySQL, and AJAX. It allows registered users to chat securely within a local network. The application uses session management, password hashing, and a modern responsive interface styled with CSS.

---

## 🎯 Project Purpose

To build a real-time messaging system that demonstrates:

- User authentication and profile management
- Real-time, dynamic message exchange using AJAX
- Secure session handling and password encryption
- Clean and intuitive UI for chat applications

---

## 🔑 Key Features

- **Secure Login & Registration**: User accounts with encrypted passwords
- **Real-Time Chat**: AJAX used for dynamic updates without page reloads
- **User Presence**: Online/offline status tracking
- **Profile Image Upload**: Users can upload avatars
- **Responsive UI**: CSS and media queries for all screen sizes

---

## 🧱 System Architecture

| Component | Technology |
|----------|-------------|
| Frontend | HTML, CSS, JavaScript |
| Backend | PHP |
| Database | MySQL |
| Server | Apache (via XAMPP/WAMP/LAMP) |

---

## 📂 Project Structure

```
📁 online-chat-app/
├── chat.php              # Main chat logic and messaging
├── index.php             # Entry point for login/registration
├── login.php             # Login authentication
├── users.php             # User list and profile info
├── header.php            # Shared layout header
├── style.css             # Styling and responsiveness
├── chatapp.sql           # Database schema
├── chat.jpeg             # Background image
└── unzipper.php          # Optional file utility
```

---

## 🧮 Core Logic

### Password Encryption:
```php
$password = password_hash($user_input, PASSWORD_DEFAULT);
```

### Chat Retrieval via AJAX:
```javascript
setInterval(() => {
  // Fetch chat messages using AJAX
}, 500);
```

---

## 🗃️ Database Schema

### `users` Table:
- `user_id`, `unique_id`, `fname`, `lname`, `email`, `password`, `img`, `status`

### `messages` Table:
- `msg_id`, `incoming_msg_id`, `outgoing_msg_id`, `msg`

---

## 🖥️ How to Use

1. Clone or download the repository.
2. Import `chatapp.sql` into MySQL using phpMyAdmin.
3. Place the project in your Apache `htdocs` folder.
4. Start Apache and MySQL using XAMPP or WAMP.
5. Open `http://localhost/online-chat-app` in your browser.
6. Register new users and start chatting!

---

## 📷 User Interface

- Login & Registration Forms
- User List with Status Indicator
- Real-Time Chat Box with Scrollable History
- Profile Picture Display

![Chat UI](chat.jpeg)

---

## 📁 Files Included

- `chat.php`, `index.php`, `login.php`, `users.php`
- `style.css`, `chatapp.sql`, `chat.jpeg`
- `README.md` (this file)

---

## 🧠 Learnings

- Implemented session and form validation in PHP
- Used AJAX to dynamically fetch messages without refreshing
- Built a UI that adapts to mobile and desktop views

---

## 🧰 Tools Used

- PHP 7.3+
- MySQL 5.7+
- Apache via XAMPP
- Visual Studio Code
- Google Chrome (testing)

---

## 🏁 Acknowledgments

This project is part of my PHP & Web Development portfolio, showcasing a real-time messaging app for local or educational deployment.

---

## 📬 Contact

For suggestions or feedback, feel free to reach out via GitHub or LinkedIn.
