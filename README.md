# 99-npx-template-React

# Getting Started with Create React App

This project was bootstrapped with [Create React App](https://github.com/facebook/create-react-app).

## Available Scripts

In the project directory, you can run:

### `npm start`

Runs the app in the development mode.\
Open [http://localhost:3000](http://localhost:3000) to view it in your browser.

The page will reload when you make changes.\
You may also see any lint errors in the console.

### `npm test`

Launches the test runner in the interactive watch mode.\
See the section about [running tests](https://facebook.github.io/create-react-app/docs/running-tests) for more information.

### `npm run build`

Builds the app for production to the `build` folder.\
It correctly bundles React in production mode and optimizes the build for the best performance.

The build is minified and the filenames include the hashes.\
Your app is ready to be deployed!

See the section about [deployment](https://facebook.github.io/create-react-app/docs/deployment) for more information.

### `npm run eject`

**Note: this is a one-way operation. Once you `eject`, you can't go back!**

If you aren't satisfied with the build tool and configuration choices, you can `eject` at any time. This command will remove the single build dependency from your project.

Instead, it will copy all the configuration files and the transitive dependencies (webpack, Babel, ESLint, etc) right into your project so you have full control over them. All of the commands except `eject` will still work, but they will point to the copied scripts so you can tweak them. At this point you're on your own.

You don't have to ever use `eject`. The curated feature set is suitable for small and middle deployments, and you shouldn't feel obligated to use this feature. However we understand that this tool wouldn't be useful if you couldn't customize it when you are ready for it.

## Learn More

You can learn more in the [Create React App documentation](https://facebook.github.io/create-react-app/docs/getting-started).

To learn React, check out the [React documentation](https://reactjs.org/).

# 🚀 99-npx-template-React

[![License: MIT](https://img.shields.io/badge/License-MIT-yellow.svg)](LICENSE) [![Build Status](https://img.shields.io/badge/build-passing-brightgreen.svg)]() [![npm version](https://img.shields.io/badge/npm-v%20--/blue.svg)]()

Minimal React starter template created with **Create React App**. Bu loyiha tezda React ilovasi qurish uchun tayyor, minimal boshlang'ich shablon.

---

## 📖 About / Loyihaning qisqacha tavsifi

`99-npx-template-React` — Create React App yordamida yaratilgan minimal template. Maqsad: yangi loyihalarni tez boshlash uchun toza va tushunarli tuzilma hamda yo‘l-yo‘riq taqdim etish.

---

## 📦 Installation / O'rnatish

```bash
# reponi klonlash
git clone https://github.com/username/99-npx-template-React.git
cd 99-npx-template-React

# node modullarini o'rnatish
npm install
```

> Agar siz `npm` o'rniga `yarn` ishlatmoqchi bo'lsangiz, `npm install` o'rniga `yarn` ishlating.

---

## ▶️ Usage / Foydalanish

```bash
# rivojlantirish serverini ishga tushirish
npm start

# testlarni ishga tushirish
npm test

# production build yaratish
npm run build

# (ehtiyotkorlik bilan) konfiguratsiyani e'lon qilish
npm run eject
```

`npm start` ishga tushganda brauzeringizda [http://localhost:3000](http://localhost:3000) ochiladi. Kodda o'zgartirishlar qilganingizda sahifa avtomatik qayta yuklanadi.

---

## 📂 Project structure / Fayl tuzilishi

```
99-npx-template-React/
├── public/            # index.html va boshqa statik fayllar
├── src/               # asosiy manba kod
│   ├── assets/        # rasmlar, shriftlar, ikonlar
│   ├── components/    # qayta ishlatiladigan UI komponentlar
│   ├── pages/         # sahifa komponentlari
│   ├── hooks/         # custom hooks
│   ├── services/      # API chaqiriqlari va util funksiyalar
│   ├── styles/        # global va modul CSS/SCSS
│   ├── App.js
│   └── index.js
├── .gitignore
├── package.json
└── README.md
```

> Ushbu strukturani o'zingizga moslab kengaytirishingiz mumkin.

---

## 🛠 Features / Funksiyalar

* ⚡ Create React App asosida tez ishga tushirish
* 🎨 Minimal va toza fayl struktura
* 🔧 ESLint va Prettier qo'shish uchun tayyor (agar siz integratsiya qilsangiz)
* 📱 Responsiv dizayn uchun tayyor joy
* 🚀 Production build optimallashtirilgan

---

## 🧰 Technologies / Texnologiyalar

* React
* JavaScript (ES6+)
* Node.js
* npm (yoki yarn)

---

## 🧩 Example: Basic App komponent

Quyida loyihada ishlatishingiz mumkin bo‘lgan juda oddiy `App.js` misoli:

```js
// src/App.js
import React from 'react';
import './styles/global.css';

function App() {
  return (
    <div className="app">
    </div>
  );
}

export default App;
```

`index.js` misoli:

```js
// src/index.js
import React from 'react';
import { createRoot } from 'react-dom/client';
import App from './App';

const container = document.getElementById('root');
const root = createRoot(container);
root.render(
  <React.StrictMode>
    <App />
  </React.StrictMode>
);
```

`global.css` misoli (`src/styles/global.css`):

```css
/* src/styles/global.css */
body {
  margin: 0;
  font-family: -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, 'Helvetica Neue', Arial;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  background: #f7f7f8;
  color: #111827;
}

.app {
  display: flex;
  min-height: 100vh;
  align-items: center;
  justify-content: center;
}

.app-header {
  text-align: center;
  padding: 2rem;
  border-radius: 12px;
  background: white;
  box-shadow: 0 6px 20px rgba(17,24,39,0.06);
}
```

---

## 🔑 Environment variables / Muhit o'zgaruvchilari

Agar siz backend URL yoki maxfiy kalitlarni saqlashni istasangiz, `.env` fayl yarating (git-ga qo'shmang). Masalan:

```
REACT_APP_API_URL=https://api.example.com
REACT_APP_OTHER_KEY=somevalue
```

> Create React App `REACT_APP_` bilan boshlangan o'zgaruvchilarni process.env orqali o'qiy oladi.

---

## 🔁 Deployment / Joylash

Build yarating va fayllarni hostingga yuklang (Netlify, Vercel, GitHub Pages va boshqalar). Misol uchun Netlify yoki Vercel bilan avtomatik CI/CD sozlash juda oson.

**Github Pages**ga deploy qilish uchun qo'shimcha paketlardan foydalanishingiz mumkin: `gh-pages`.

---

## 🤝 Contribution / Hissa qo'shish

Agar loyiha ochiq bo'lsa va sizga hissa qo'shish qulay bo'lsa:

1. Fork qiling
2. Yangi branch yarating: `git checkout -b feature/your-feature`
3. O'zgartirishlarni qiling va commit qiling
4. Push qiling va Pull Request oching

Iltimos, kod standartlariga rioya qiling va unit testlar qo'shishni o'ylab ko'ring.

---

## 🐛 Issues / Muammolar

Muammolarni `Issues` bo'limida oching — iloji boricha batafsil tavsif va reproduksiya bosqichlarini yozing.

---

## 📌 To-Do / Kelajak rejalar

* [ ] Routing qo'shish (React Router)
* [ ] State management (Context API yoki Redux Toolkit)
* [ ] Unit va integration testlar (Jest + React Testing Library)
* [ ] UI kit yoki Tailwind integratsiyasi

---

## 📄 License / Litsenziya

This project is licensed under the MIT License - see the [LICENSE](LICENSE) file for details.

---

## ✉️ Contact

Agar savollar bo'lsa: `yourname@example.com` yoki GitHub profil orqali murojaat qiling.

---

> Agar xohlasangiz, men README faylini: badge'lar bilan to'ldirib, `LICENSE` va `CODE_OF_CONDUCT` fayllarini ham yaratib beraman. Shuningdek, agar sizga to'liq React loyiha fayllari (src, public) kerak bo'lsa, men ularni ham tayyorlab bera olaman — qaysi variantni xohlaysiz?
