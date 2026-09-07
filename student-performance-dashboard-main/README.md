# 🎓 Northstar Study - Student Performance Dashboard

A modern, interactive web-based dashboard for tracking and analyzing student performance signals, predictions, and learning pathways.

## 📋 Project Overview

**Northstar Study** is a comprehensive student performance signal platform that helps educators:
- Visualize real-time student performance metrics
- Generate predictive outcomes based on current trends
- Track attendance and engagement patterns
- Explore learning pathways and support strategies
- Access student notes and progress tracking

## 🛠️ Prerequisites

Before you begin, make sure you have the following installed:

- **Node.js** (v16.x or higher) - [Download here](https://nodejs.org/)
- **npm** (v7.x or higher) - Usually comes with Node.js
- **Git** (optional, for cloning the repository)

To check if you have these installed, run:
```bash
node --version
npm --version
```

## 📦 Installation Steps

### Step 1: Navigate to Project Directory
```bash
cd student-performance-dashboard-main
```

### Step 2: Install Dependencies
The project uses npm with legacy peer dependency support due to some version conflicts:

```bash
npm install --legacy-peer-deps
```

This installs all required packages including:
- React & React DOM
- TypeScript
- Vite (build tool)
- Tailwind CSS (styling)
- Recharts (charting library)
- And more...

**Note:** You may see some deprecation warnings - these are safe to ignore.

## 🚀 Running the Dashboard

### Start Development Server
```bash
npm run dev
```

You should see output similar to:
```
  VITE v7.3.6  ready in 7145 ms

  ➜  Local:   http://localhost:3000/
  ➜  Network: http://10.239.97.16:3000/
  ➜  press h + enter to show help
```

### Access the Dashboard
Open your web browser and navigate to:
```
http://localhost:3000/
```

## 📱 Dashboard Features

### Sidebar Navigation
- **Overview** - Dashboard home with key performance signals
- **Predictor** - View predicted student outcomes and weighted factors
- **Pathways** - Explore learning pathways and support strategies
- **Notes** - Access and manage student notes
- **Settings** - Configure dashboard preferences

### Key Metrics Displayed
- **Predicted Outcome** - AI-powered prediction with recent trend (+/- points)
- **Current Average** - Student's current class standing (above/below median)
- **Attendance** - Attendance tracking with steady/changing indicators
- **Support Status** - Overall support level and recommendations

### Student Information
- Student name and grade level
- Group assignment
- Teacher account information
- Quick access to settings and account options

## 🔧 Available Commands

| Command | Description |
|---------|-------------|
| `npm run dev` | Start the development server |
| `npm run build` | Build for production |
| `npm run preview` | Preview production build |
| `npm audit fix` | Fix security vulnerabilities (optional) |

## 📂 Project Structure

```
student-performance-dashboard-main/
├── client/                    # Frontend React application
│   ├── src/
│   │   ├── components/       # Reusable React components
│   │   ├── pages/            # Page components
│   │   ├── contexts/         # React context (Theme, etc.)
│   │   ├── hooks/            # Custom React hooks
│   │   ├── lib/              # Utility functions
│   │   └── App.tsx           # Root component
│   └── index.html            # HTML entry point
├── server/                    # Backend/API server
├── report/                    # Report generation assets
├── qr/                        # QR code assets
├── package.json              # Project dependencies
├── vite.config.ts            # Vite configuration
└── tsconfig.json             # TypeScript configuration
```

## 🎨 Technology Stack

- **Frontend Framework:** React + TypeScript
- **Build Tool:** Vite (Fast and optimized)
- **Styling:** Tailwind CSS + Custom CSS
- **Charts:** Recharts
- **Routing:** Wouter
- **UI Components:** Custom component library
- **Theme:** Dark/Light theme support

## 🐛 Troubleshooting

### Issue: `npm install` fails with peer dependency errors
**Solution:** Use the legacy peer deps flag:
```bash
npm install --legacy-peer-deps
```

### Issue: Port 3000 is already in use
**Solution:** Either stop the process using port 3000, or modify `vite.config.ts` to use a different port.

### Issue: Page shows loading errors (404 or 500)
**Solution:** 
1. Check that the dev server is running
2. Clear browser cache (Ctrl+Shift+Delete)
3. Hard refresh the page (Ctrl+Shift+R)
4. Check browser console for specific errors

### Issue: Styles not loading properly
**Solution:** 
1. Restart the dev server
2. Clear node_modules and reinstall: `rm -r node_modules && npm install --legacy-peer-deps`

## 📝 Notes

- The dashboard uses mock/sample data for demonstration
- Changes made in development are automatically hot-reloaded
- The project includes TypeScript for type safety
- Tailwind CSS is used for responsive, utility-first styling

## 🤝 Development Tips

1. **Hot Module Replacement (HMR):** Changes to files are automatically reflected in the browser
2. **TypeScript:** The project uses TypeScript for better code quality
3. **Component System:** Modular component architecture in `client/src/components/`
4. **Responsive Design:** Dashboard is mobile-friendly and responsive

## 📄 License

This project is part of the Northstar Study initiative.

## ✨ Quick Start Summary

```bash
# 1. Navigate to the project
cd student-performance-dashboard-main

# 2. Install dependencies
npm install --legacy-peer-deps

# 3. Start the server
npm run dev

# 4. Open browser
# Visit: http://localhost:3000/
```

That's it! Your dashboard should be up and running! 🎉

---

**For more help or issues, check the browser console (F12) for detailed error messages.**
