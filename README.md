# 🔗 URL Shortener & QR Code Generator

A lightweight, single-file web app that lets you **shorten URLs using the Bitly API** and **generate QR codes instantly** — all built inside **one HTML file** using HTML, CSS, and JavaScript.

---

## 🚀 Features

* 🔗 Shorten long URLs via Bitly API
* 📱 Generate QR codes for shortened links
* 📄 Single-file project (no dependencies or setup needed)
* 🎨 Clean UI with embedded CSS
* ⚡ Fast and easy to use

---

## 🛠️ Tech Stack

* **HTML5** – Structure
* **CSS3 (inline)** – Styling
* **JavaScript (inline)** – Logic & API calls
* **Bitly API** – URL shortening
* **QR Code API / Library** – QR generation

---

## 📂 Project Structure

```id="j2k9dl"
index.html   # Contains HTML, CSS, and JavaScript
```

---

## ⚙️ Setup & Usage

1. **Download or Clone the Repository**

   ```bash
   git clone https://github.com/your-username/url-shortener-qr.git
   cd url-shortener-qr
   ```

2. **Get Your Bitly API Token**

   * Go to https://bitly.com/
   * Log in → Settings → API
   * Generate an access token

3. **Add Token to Code**
   Open `index.html` and find:

   ```javascript
   const BITLY_TOKEN = "YOUR_ACCESS_TOKEN";
   ```

   Replace with your actual token.

4. **Run the App**

   * Just open `index.html` in your browser
   * No server or installation required 🎉

---

## 🔧 How It Works

1. Enter a long URL
2. Click the **Shorten** button
3. App sends request to Bitly API
4. Displays shortened URL
5. Automatically generates QR code

---

## 📌 Example API Call

```javascript id="b7m2qs"
fetch("https://api-ssl.bitly.com/v4/shorten", {
  method: "POST",
  headers: {
    "Authorization": `Bearer ${BITLY_TOKEN}`,
    "Content-Type": "application/json"
  },
  body: JSON.stringify({
    long_url: userInputURL
  })
})
```

---

## 💡 Future Improvements

* 📋 Copy-to-clipboard button
* 📥 Download QR code
* 🌙 Dark mode
* 📊 Analytics (Bitly stats)

---

## 📄 License

This project is licensed under the **MIT License**.

---

## ⭐ Support

If you found this useful, give the repo a ⭐ on GitHub!

---
