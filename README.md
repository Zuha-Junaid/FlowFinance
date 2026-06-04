# 💸 FlowFinance

> A modern, beautiful personal finance tracker — track income, expenses, and visualize your financial health. Built with React + Vite + Tailwind CSS.

![FlowFinance](https://img.shields.io/badge/FlowFinance-Personal%20Finance%20Tracker-22c55e?style=for-the-badge&logo=react)
![React](https://img.shields.io/badge/React-18-61DAFB?style=flat-square&logo=react)
![Vite](https://img.shields.io/badge/Vite-5-646CFF?style=flat-square&logo=vite)
![TailwindCSS](https://img.shields.io/badge/Tailwind-3-06B6D4?style=flat-square&logo=tailwindcss)
![License](https://img.shields.io/badge/License-MIT-green?style=flat-square)

---

## 🌐 Live Demo

🔗 **[flowfinance.netlify.app](https://flowfinance.netlify.app)**

---

## 📸 Screenshots

| Dashboard | Transactions |
|-----------|-------------|
| <img width="1168" height="731" alt="image" src="https://github.com/user-attachments/assets/af70c79d-7655-4c9e-a485-fc3171957232" />
 |<img width="1165" height="740" alt="image" src="https://github.com/user-attachments/assets/dbd56ea1-4c94-48fc-95b8-08bd881f0b40" />
 |

---

## ✨ Features

- 🔐 **Authentication** — Register, login, forgot password, reset password
- 📊 **Dashboard** — Live balance, income & expense summary cards
- 📈 **Charts** — Monthly area chart + spending breakdown donut chart
- 💳 **Transactions** — Add, edit, delete income and expense records
- 🔍 **Search & Filter** — Search by description, filter by type, sort by date or amount
- 📄 **PDF Report** — Download a full financial report as a professional PDF
- 💾 **Persistent Storage** — All data saved locally, no backend required
- 📱 **Fully Responsive** — Works on mobile, tablet, and desktop

---

## 🛠️ Tech Stack

| Technology | Purpose |
|------------|---------|
| [React 18](https://react.dev) | UI framework |
| [Vite 5](https://vitejs.dev) | Build tool & dev server |
| [Tailwind CSS 3](https://tailwindcss.com) | Styling |
| [React Router v6](https://reactrouter.com) | Client-side routing |
| [Recharts](https://recharts.org) | Charts & data visualization |
| [jsPDF](https://github.com/parallax/jsPDF) | PDF report generation |
| [Lucide React](https://lucide.dev) | Icons |
| [date-fns](https://date-fns.org) | Date formatting |

---

## 🚀 Getting Started

### Prerequisites
- Node.js v18 or higher → [Download](https://nodejs.org)
- npm v9 or higher (comes with Node.js)

### Installation

```bash
# 1. Clone the repository
git clone https://github.com/yourusername/flowfinance.git

# 2. Navigate into the project
cd flowfinance

# 3. Install dependencies
npm install

# 4. Start the development server
npm run dev
```

Open **http://localhost:5173** in your browser. 🎉

### Build for Production

```bash
npm run build
```

The production-ready files will be in the `dist/` folder.

---

## 📁 Project Structure

```
flowfinance/
├── index.html
├── package.json
├── vite.config.js
├── tailwind.config.js
├── postcss.config.js
└── src/
    ├── App.jsx                          # Root component with routing
    ├── main.jsx                         # React entry point
    ├── index.css                        # Global styles + Tailwind
    ├── context/
    │   ├── AuthContext.jsx              # Authentication state
    │   └── TransactionContext.jsx       # Transaction data & logic
    ├── components/
    │   ├── Layout.jsx                   # Sidebar + mobile nav
    │   ├── AuthCard.jsx                 # Auth pages wrapper
    │   ├── StatCard.jsx                 # Summary stat cards
    │   └── TransactionModal.jsx         # Add/Edit modal
    ├── pages/
    │   ├── LoginPage.jsx
    │   ├── RegisterPage.jsx
    │   ├── ForgotPasswordPage.jsx
    │   ├── ResetPasswordPage.jsx
    │   ├── DashboardPage.jsx
    │   └── TransactionsPage.jsx
    └── utils/
        └── generateReport.js            # PDF export utility
```

---

## 📄 Pages & Routes

| Route | Page | Access |
|-------|------|--------|
| `/login` | Login | Public |
| `/register` | Register | Public |
| `/forgot-password` | Forgot Password | Public |
| `/reset-password` | Reset Password | Public |
| `/` | Dashboard | Private |
| `/transactions` | Transactions | Private |

---

## 🔒 How Authentication Works

FlowFinance uses **localStorage** for authentication — no backend or database required.

- User accounts are stored in `localStorage` under key `ff_users`
- Active session stored under `ff_session`
- Each user's transactions stored under `ff_txns_{userId}`
- All data is private to the user's browser

---

## 📊 How to Use

1. **Register** a new account at `/register`
2. You'll be automatically logged in and taken to the **Dashboard**
3. The dashboard is pre-loaded with **15 sample transactions** so you can explore
4. Click **"Add Transaction"** to add your own income or expense
5. Go to **Transactions** to view, edit, search, filter, and delete records
6. Click **"Download Report"** on the dashboard to export a PDF of your finances
7. Click the logout icon in the sidebar to sign out

---

## 🤝 Contributing

Contributions are welcome! Feel free to:

1. Fork the repository
2. Create a new branch: `git checkout -b feature/your-feature`
3. Make your changes and commit: `git commit -m "Add your feature"`
4. Push to your branch: `git push origin feature/your-feature`
5. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License** — you are free to use, modify, and distribute it.

---

## 👨‍💻 Author

Built with ❤️ using React + Vite + Tailwind CSS

⭐ **If you found this useful, please give it a star on GitHub!**

---

*FlowFinance — Take control of your finances*
