# Archives de Canada 🇨🇦

[![Version](https://img.shields.io/badge/version-5.0-8b2626.svg?style=flat-square)](https://github.com)
[![License](https://img.shields.io/badge/license-MIT-blue.svg?style=flat-square)](LICENSE)
[![Build Status](https://img.shields.io/badge/status-active-success.svg?style=flat-square)](https://github.com)
[![PRs Welcome](https://img.shields.io/badge/PRs-welcome-brightgreen.svg?style=flat-square)](CONTRIBUTING.md)

> **National Directory of Global Journalism & Media // Répertoire national du journalisme et des médias mondiaux**

**Archives de Canada** is a lightweight, zero-dependency, web-based intelligence matrix and bilingual media directory. Built with a refined archival aesthetic, it preserves public access to verified Canadian and international news outlets while providing a universal interactive execution workspace via **World Direct Hub v5**.

---

## 📸 Key Features & Capabilities

- 🇨🇦 **Bilingual Core (EN / FR):** Instant toggle between English and French interface localizations.
- 📰 **Curated Media Directory:** Comprehensive index of top Canadian, North American, European, African, Asian, and Oceanian news organizations.
- ⚡ **World Direct Hub v5:** Built-in interactive iframe execution canvas to launch, inspect, and read live news articles directly within the app.
- ⭐️ **Local Storage Favourites & Sync:** Bookmark essential outlets with instant local storage persistence, complete with JSON export/import capabilities.
- 🌙 **Archival Light & Dark Modes:** Carefully crafted typography utilizing Google Fonts (*Cinzel*, *Newsreader*, *Inter*) with dynamic theme switching.
- 📱 **Fully Responsive Layout:** Optimized for mobile viewports, tablets, and desktop workstations via Tailwind CSS.
- 🔒 **Privacy First:** Zero tracking, zero telemetry, and zero backend required. All preferences stay entirely on the user's local device.

---

## 🛠 Tech Stack

| Component | Technology |
| :--- | :--- |
| **Markup & Layout** | HTML5 / Tailwind CSS (CDN) |
| **Typography** | Google Fonts (*Cinzel*, *Newsreader*, *Inter*) |
| **Iconography** | FontAwesome 6.4.0 (Free CDN) |
| **Scripting & Logic** | Pure Vanilla JavaScript (ES6+) |
| **Data Storage** | Native `localStorage` API |

---

## 🚀 Quick Start

Because **Archives de Canada** is engineered as a standalone single-file web application, no build tools or package managers (NPM/Yarn) are strictly required.

### Method 1: Local Launch

1. Clone the repository:
   ```bash
   git clone https://github.com/your-username/archives-de-canada.git
   ```
2. Navigate into the directory:
   ```bash
   cd archives-de-canada
   ```
3. Open `index.html` in any modern web browser:
   ```bash
   # On macOS
   open index.html

   # On Windows
   start index.html

   # On Linux
   xdg-open index.html
   ```

### Method 2: Local HTTP Server (Optional)

For the best experience when working with frame execution and browser security headers:
```bash
# Using Python 3
python -m http.server 8000

# Using Node npx
npx serve .
```
Then navigate to `http://localhost:8000` in your web browser.

---

## 📁 Repository Structure

```
archives-de-canada/
├── index.html         # Complete single-file application bundle
├── README.md          # Project documentation
└── LICENSE            # Open-source license (MIT)
```

---

## 📖 Usage Guide

### 1. Searching & Filtering Outlets
* **Search Bar:** Query by outlet name, country, region, or broadcast language.
* **Region Pills:** Quickly filter outlets by region (`Canada`, `United States`, `Europe`, `Africa`, `Asia`, `Oceania`, `International`).
* **Favourites Filter:** Toggle the star icon or choose the `Favourites` filter to isolate bookmarked news sources.

### 2. Executing News via World Direct Hub
1. Scroll down to the **World Direct Hub** section.
2. Enter any news article URL or select one of the **Global Outlets Quick Launch** preset buttons.
3. Click **Execute News** (`⚡`) to load the target link inside the interactive frame.
4. If a target domain enforces strict `X-Frame-Options` or `Content-Security-Policy` header restrictions, click **Open Direct** to view the article in a clean tab.

### 3. Exporting & Importing Favourites
1. Open the **Favourites Drawer** from the top navbar.
2. Click **Export** to generate a local `.json` file (`archives_de_canada_favourites.json`).
3. Click **Import** on any secondary device to restore your starred news directories instantly.

---

## ⚙️ Configuration & Customization

To add additional news outlets to the directory, update the `mediaOutlets` array inside the `<script>` block in `index.html`:

```javascript
{
    id: "your-outlet-id",
    name: "Outlet Name",
    region: "Canada", // Region classification
    country: "Canada",
    language: "EN",
    description: "Brief summary of the news outlet focus.",
    url: "https://example.com/news",
    iconClass: "fa-solid fa-newspaper"
}
```

---

## 🤝 Contributing

Contributions, issue reports, and media directory submissions are welcome!

1. Fork the Project.
2. Create your Feature Branch (`git checkout -b feature/NewMediaOutlet`).
3. Commit your Changes (`git commit -m 'Add new regional media source'`).
4. Push to the Branch (`git push origin feature/NewMediaOutlet`).
5. Open a Pull Request.

---

## 📄 License

Distributed under the **MIT License**. See `LICENSE` for more information.

---

<p align="center">
  <i>Archives de Canada • Preserving bilingual press access and open global journalism.</i>
</p>
