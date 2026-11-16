# SkillBridge Frontend Web Application

Modern, industry-grade React single-page application (SPA) for **SkillBridge – Online Learning & Skill Development Platform**, powered by **React 18**, **Vite**, **Tailwind CSS**, **Recharts**, and **Lucide React**.

---

## 🚀 Features

- **Responsive Learning Platform**: Modern UI/UX with smooth transitions, responsive navigation, and accessible layout.
- **Role-Based Interfaces**:
  - **Student Portal**: Course browsing, interactive video player, real-time progress saving, interactive quizzes, assignment submission, PDF certificate verification & download.
  - **Instructor Portal**: Course creation wizard, curriculum builder (sections & lessons), quiz creator, assignment evaluator, grading dashboard, student performance metrics.
  - **Admin Control Center**: Platform analytics, user management (ban/activate/edit roles), course approval/rejection, category management.
- **Data Visualization**: Recharts integration for student progress tracking, instructor revenue analytics, and admin platform KPIs.
- **Production-Ready**: Preconfigured with Vite production bundling, Tailwind CSS, and Axios interceptors for automatic JWT authentication.

---

## 🛠 Tech Stack

- **Framework**: React 18
- **Build Tool**: Vite
- **Styling**: Tailwind CSS, PostCSS, Autoprefixer
- **Icons**: Lucide React
- **Charts**: Recharts
- **Routing**: React Router DOM (v6)
- **HTTP Client**: Axios with automatic JWT bearer token interceptors

---

## 📦 Getting Started

### 1. Prerequisites
- Node.js (v18 or higher)
- npm or yarn

### 2. Installation
```bash
# Clone the repository
git clone https://github.com/saranyak2406/frontend.git
cd frontend

# Install dependencies
npm install
```

### 3. Environment Variables
Create a `.env` file in the root directory:
```env
# Point to your SkillBridge backend REST API
VITE_API_URL=https://backend-n73l.onrender.com/api
```
*(For local backend development, set `VITE_API_URL=http://localhost:5000/api`)*

### 4. Running the Development Server
```bash
npm run dev
```
Open [http://localhost:5173](http://localhost:5173) in your browser.

### 5. Production Build
```bash
# Build optimized production bundle
npm run build

# Preview the production build locally
npm run preview
```

---

## ☁️ Deploying on Render (Static Site)

1. Go to [Render Dashboard](https://dashboard.render.com) and click **New +** → **Static Site**.
2. Connect this repository: `https://github.com/saranyak2406/frontend.git`.
3. Configure the deployment settings:
   - **Root Directory**: *(leave blank — repository root)*
   - **Build Command**: `npm install && npm run build`
   - **Publish Directory**: `dist`
4. Configure **Redirects/Rewrites** (for client-side React Router routing):
   - **Type**: `Rewrite`
   - **Source**: `/*`
   - **Destination**: `/index.html`
5. Environment Variables:
   - `VITE_API_URL`: `https://backend-n73l.onrender.com/api`
6. Click **Create Static Site**.

---

## ☁️ Deploying on Vercel or Netlify

- **Framework Preset**: Vite
- **Build Command**: `npm run build`
- **Output Directory**: `dist`
- **Environment Variable**: `VITE_API_URL=https://backend-n73l.onrender.com/api`

---

## 📄 License
MIT
