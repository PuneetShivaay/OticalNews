# 📰 OticalNews React App

[![License: GPL-3.0](https://img.shields.io/badge/License-GPL--3.0-blue.svg?style=flat-square)](LICENSE)
[![React](https://img.shields.io/badge/Frontend-React.js-61DAFB?style=flat-square&logo=react&logoColor=black)](https://reactjs.org/)
[![JavaScript](https://img.shields.io/badge/Language-JavaScript-F7DF1E?style=flat-square&logo=javascript&logoColor=black)](https://developer.mozilla.org/en-US/docs/Web/JavaScript)
[![NewsAPI](https://img.shields.io/badge/Data_Source-NewsAPI-FF6B6B?style=flat-square)](https://newsapi.org/)

A feature-rich news browsing web application built with React.js. OticalNews fetches and categorizes real-time global news headlines across multiple domains using NewsAPI.

---

## 📸 Preview

![image](https://github.com/user-attachments/assets/b40e28fe-a7a1-48f5-a915-eeb54d2b417e) 
---

## ✨ Features

- 📑 **Category-Based Filtering:** Browse top headlines filtered by categories including Business, Entertainment, General, Health, Science, Sports, and Technology.
- 🖼️ **Responsive Article Cards:** Clean card layouts displaying titles, descriptions, publication dates, source badges, and direct links to original stories.
- ⏳ **Loading Spinners:** Custom asynchronous loading indicator (`Spinner.js` / `Loading.gif`) between category transitions and page requests.
- 🧪 **Offline / Mock Testing:** Includes `sampleOutput.json` for development without exhausting live API request limits.

---

## ⚠️ Important Note on Deployment & NewsAPI

> **Localhost Only:** The free developer tier of [NewsAPI.org](https://newsapi.org/) restricts requests exclusively to **`localhost`**. Requests originating from hosted URLs (e.g., GitHub Pages, Vercel, Netlify) will be blocked with a `426 Upgrade Required` or CORS error.
> 
> To deploy this project to production, you will need either:
> 1. A paid commercial plan from NewsAPI, or
> 2. An alternative free news API that allows hosted origins (such as GNews or Currents API), or
> 3. A serverless proxy/backend middleware to forward requests.

---

## 📂 Project Structure

```text
OticalNews/
├── public/
│   ├── favicon.ico
│   ├── index.html
│   └── manifest.json
├── src/
│   ├── components/
│   │   ├── NavBar.js          # Navigation bar with category routing
│   │   ├── News.js            # Main news container handling API fetching & pagination
│   │   ├── NewsItem.js        # Individual article card UI
│   │   └── Spinner.js         # Loading indicator component
│   ├── App.js                 # App configuration & routing
│   ├── App.css                # App-level styling
│   ├── Loading.gif            # Spinner asset
│   ├── sampleOutput.json      # Mock response payload for offline dev
│   └── index.js               # React DOM entry point
├── package.json
└── README.md
```

---

## 🛠️ Tech Stack

- **Framework:** React.js
- **Styling:** CSS3 / Bootstrap
- **API:** [NewsAPI.org](https://newsapi.org/)
- **Runtime:** Node.js & npm

---

## 🚀 Getting Started Locally

### Prerequisites
- Node.js (v14 or higher)
- npm
- Free API Key from [NewsAPI.org](https://newsapi.org/)

### 1. Clone the Repository
```bash
git clone https://github.com/PuneetShivaay/OticalNews.git
cd OticalNews
```

### 2. Install Dependencies
```bash
npm install
```

### 3. Configure Your NewsAPI Key
Add your API key where appropriate (e.g., in `App.js` or via a `.env.local` file):
```env
REACT_APP_NEWS_API_KEY=your_news_api_key_here
```

### 4. Start the Application
```bash
npm start
```
Runs the app in development mode at [http://localhost:3000](http://localhost:3000).

---

## 📄 License

This project is licensed under the **GNU General Public License v3.0** — see the [LICENSE](LICENSE) file for details.
