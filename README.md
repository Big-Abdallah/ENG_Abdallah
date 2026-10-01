# 👨‍💻 Abdallah Mohamed — Portfolio

My personal portfolio website: a Full Stack Developer, backend-focused (Node.js), and Computer Science student at FCIS, Mansoura University.

🔗 **Live site:** [eng-abdallah-ten.vercel.app](https://eng-abdallah-ten.vercel.app/)

---

## ✨ Features

- 🌗 **Light and dark mode** with a toggle
- 🌍 **English and Arabic** with full **RTL** layout support
- 🧩 **Bento-style card layout** with rounded cards, pill buttons, and smooth hover motion
- 🎞️ **Scroll-reveal animations** built with the Intersection Observer API (no animation library)
- 📱 **Fully responsive** with a floating pill navbar and a mobile menu
- 🎓 **Training section** with a clickable certificate preview
- 🔎 Basic SEO: page title, meta description, and `sitemap.xml`

---

## 📄 Sections

| Section       | What it shows                                                                    |
| ------------- | -------------------------------------------------------------------------------- |
| **Hero**      | Name, role, short intro, and quick links                                         |
| **About**     | Background, education, and focus on backend development                          |
| **Skills**    | Backend, Frontend, Databases, and Tools, grouped as chips                        |
| **Training**  | 300-hour Full Stack Web Development diploma at Route Academy, with certificate   |
| **Projects**  | Case studies with tech tags and GitHub links                                     |
| **Contact**   | Email, location, LinkedIn, and GitHub                                            |

---

## 🚀 Featured Projects

| Project                  | Type       | Stack                                            |
| ------------------------ | ---------- | ------------------------------------------------ |
| **Sara7a**               | Backend    | Node.js, Express, MongoDB, Redis, JWT            |
| **LOOP**                 | Frontend   | React, Tailwind CSS, Hero UI, React Router, Zod  |
| **E-Commerce Platform**  | Backend    | React, Node.js, Express, MongoDB, JWT            |
| **Note App**             | Frontend   | React, Tailwind CSS, React Hook Form, Zod, JWT   |
| **Weather Dashboard**    | Frontend   | React, Tailwind CSS, wttr.in API                 |

---

## 🛠️ Tech Stack

| Category   | Tools                         |
| ---------- | ----------------------------- |
| Framework  | React 19, Vite 7              |
| Styling    | Tailwind CSS 4                |
| Icons      | Lucide React                  |
| Linting    | ESLint 9                      |
| Deployment | Vercel                        |

---

## 📁 Project Structure

```
├── public/
│   └── sitemap.xml
├── src/
│   ├── assets/           # Profile photo, certificate, icon
│   ├── Portfolio.jsx     # Whole site: theme + language contexts, translations,
│   │                     # sections (Navbar, Hero, About, Skills, Training,
│   │                     # Projects, Contact, Footer)
│   ├── App.jsx
│   ├── main.jsx
│   └── index.css
├── index.html
├── vercel.json           # SPA rewrite
└── package.json
```

---

## 🧱 How It Works

- **Theme:** a `ThemeContext` holds the dark/light state, and a `getColors(dark)` helper returns the matching Tailwind classes.
- **Language:** a `LangContext` holds the active language and a `TRANSLATIONS` object (`en` / `ar`). Switching language also flips the page direction (`ltr` / `rtl`).
- **Content:** skills, training stages, projects, and contact info are built from the translation object, so adding a language or editing text happens in one place.

### Adding a project

Add a description to both languages in `TRANSLATIONS.*.projectDescriptions`, then add an entry to `getProjects(t)`:

```js
{
  title: "My Project",
  type: t.projectTypes.frontend,
  description: t.projectDescriptions.myProject,
  tags: ["React", "Tailwind CSS"],
  githubUrl: "https://github.com/Big-Abdallah/my-project",
}
```

---

## ⚙️ Getting Started

### Prerequisites

- [Node.js](https://nodejs.org/) v20.19 or higher
- npm

### Installation

```bash
git clone https://github.com/Big-Abdallah/ENG_Abdallah.git
cd ENG_Abdallah
npm install
```

### Run in development

```bash
npm run dev
```

### Build for production

```bash
npm run build
npm run preview
```

---

## 📜 Available Scripts

| Script            | Description                           |
| ----------------- | ------------------------------------- |
| `npm run dev`     | Start the development server          |
| `npm run build`   | Build the app for production          |
| `npm run preview` | Preview the production build locally  |
| `npm run lint`    | Run ESLint                            |

---

## 📬 Contact

- 📧 Email: [swe.abdallah.m@icloud.com](mailto:swe.abdallah.m@icloud.com)
- 💼 LinkedIn: [engabdallahmohamed](https://www.linkedin.com/in/engabdallahmohamed/)
- 🐙 GitHub: [@Big-Abdallah](https://github.com/Big-Abdallah)
- 📍 Dakahlia, Egypt

---

## 📄 License

No license has been added yet. Add a `LICENSE` file (e.g., MIT) to specify the terms. Note that the profile photo and certificate are personal and not intended for reuse.
