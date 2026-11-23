
<div align="center">

# 📊 Sales Dashboard

**A fully functional, single-file admin dashboard built with pure HTML, CSS & JavaScript — no frameworks, no build tools.**

![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS3](https://img.shields.io/badge/CSS3-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Chart.js](https://img.shields.io/badge/Chart.js-FF6384?style=for-the-badge&logo=chartdotjs&logoColor=white)
![License](https://img.shields.io/badge/License-MIT-green?style=for-the-badge)

</div>

---

## 📖 Overview

**Sales Dashboard** is a modern, responsive, feature-rich analytics dashboard packed into a **single HTML file**. It includes interactive charts, a fully sortable & filterable data table, a task manager, dark/light theme, and more — perfect as a starter template for admin panels, SaaS dashboards, or portfolio projects.

## ✨ Features

### 📈 Charts & Visualizations (powered by Chart.js)
- 💰 **Revenue Overview** — animated line/area chart with gradient fills + range switcher (7D / 30D / 12M)
- 🍩 **Traffic Sources** — doughnut chart with custom center-text plugin
- 📊 **Sales by Category** — gradient bar chart
- 🕸️ **Team Performance** — radar chart (this year vs last year)
- ⚡ **Mini sparklines** inside every KPI card

### 🧩 Dashboard Functionality
- 🌙 **Dark / Light mode** — persisted in `localStorage`, charts re-render on theme change
- 🔍 **Orders table** — live search, status filter, sortable columns (↑↓), pagination, rows-per-page selector
- 👁️ **Row actions** — view order details & delete rows
- ✅ **Task Manager** — add / complete / delete tasks with a live progress bar (saved in `localStorage`)
- 🔔 **Notifications dropdown** with mark-all-read
- 👤 **Profile dropdown** menu
- 🔢 **Animated counting** KPI numbers
- 🔄 **Refresh button** — randomizes & updates all chart data
- 📄 **Export Report** — downloads real orders data as CSV
- 🔔 **Toast notifications** system
- 📱 **Fully responsive** — collapsible sidebar on desktop, off-canvas sidebar on mobile

## 🛠️ Tech Stack

| Tool | Purpose |
|------|---------|
| HTML5 | Structure (single file) |
| CSS3 | Theming via CSS variables, grid/flexbox, responsive design |
| Vanilla JavaScript (ES6+) | All logic — zero frameworks |
| [Chart.js v4](https://www.chartjs.org/) | All charts (loaded via CDN) |
| Inline SVG sprite | All icons (no icon library needed) |

## 🚀 Getting Started

No installation or build steps required. 

### Option 1 — Direct
1. Download / clone the repo
2. Open `index.html` in any modern browser

```bash
git clone https://github.com/khdcoder/sales-dashboard.git
cd sales-dashboard
# then open index.html in your browser
```

> ⚠️ An internet connection is needed the first time (Chart.js CDN + Google Fonts). Everything else works fully offline.

### Option 2 — Live server (recommended for development)
```bash
npx serve .
# or
python -m http.server 8000
```

## 📁 Project Structure

```
sales-dashboard/
├── index.html      # Entire app — HTML + CSS + JS in one file
└── README.md
```

## 🎨 Customization

Everything is easy to tweak inside `index.html`:

| What | Where |
|------|-------|
| **Color theme** | `:root` and `[data-theme="dark"]` CSS variables |
| **KPI numbers** | `data-count`, `data-prefix`, `data-suffix` attributes on `.stat-value` |
| **Chart data** | `revData`, `catData`, and the chart configs inside `buildCharts()` |
| **Orders data** | The `orders` array in the `<script>` section |
| **Tasks data** | The `tasks` array (auto-saved to `localStorage` key `nova_tasks`) |
| **Sidebar / branding** | The `.sidebar` markup & `.brand-name` text |
| **Theme key** | `localStorage` key `nova_theme` (search for it if renaming) |

## 🖼️ Preview

<img width="1360" height="642" alt="image" src="https://github.com/user-attachments/assets/cc42fa5a-433e-49e2-8d33-91a4f0bd9bfa" />


## 🌐 Browser Support

| Browser | Support |
|---------|---------|
| Chrome / Edge (latest) | ✅ Full |
| Firefox (latest) | ✅ Full |
| Safari (latest) | ✅ Full |
| IE 11 | ❌ Not supported |

## 🗺️ Roadmap

- [ ] Multi-page sections (Orders / Customers / Products views)
- [ ] Connect to a real REST API / database
- [ ] Chart export as PNG
- [ ] User authentication flow
- [ ] Drag-and-drop dashboard widgets

## 🤝 Contributing

Contributions are welcome! 
1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

## 👤 Author

**khdcoder**

- GitHub: [@khdcoder](https://github.com/khdcoder)

---

<div align="center">

⭐ **If this dashboard helped you, please consider giving it a star!** ⭐

</div>
