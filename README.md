# DevLink — Full-Stack Developer Networking Platform

**Discover developers. Share skills. Build connections.**

DevLink is a full-stack developer networking project built with **Next.js (App Router), TypeScript, Tailwind CSS, Prisma ORM, and Neon PostgreSQL**. Inspired by developer portfolios and professional networking platforms, it provides a central place to create developer profiles, discover other developers, and explore their skills and links.

> **Project type:** Personal full-stack development project  
> **Developed:** May 2026  
> **Deployment:** Vercel

### 🔗 Links

- **Live demo:** [build-dev-link-platform.vercel.app](https://build-dev-link-platform.vercel.app/)
- **Source code:** [Devlink-Developer-Network](https://github.com/p-g-udara-dilshan/Devlink-Developer-Network)

## ✨ Features

- **Developer profiles:** Create and manage profiles containing developer information, skills, and relevant links.
- **Developer directory:** Browse a collection of developer profiles.
- **Search and filtering:** Find developers by name, username, or technical skills.
- **Dynamic profile pages:** Open individual developer profiles through dynamic Next.js routes.
- **Server-side workflows:** Use Next.js Server Actions for application data operations.
- **Database persistence:** Model and access developer data with Prisma ORM and PostgreSQL hosted on Neon.
- **Responsive interface:** Tailwind CSS layouts designed for different screen sizes.

## 🛠️ Technology Stack

| Layer | Technology |
| --- | --- |
| Full-stack framework | Next.js (App Router) |
| Language | TypeScript |
| Styling | Tailwind CSS |
| Server-side operations | Next.js Server Actions |
| ORM | Prisma |
| Database | PostgreSQL (Neon) |
| Deployment | Vercel |

## 🏗️ How It Works

1. Developers interact with profile and discovery pages in the Next.js interface.
2. Application server-side operations use Server Actions where appropriate.
3. Prisma provides typed access to the PostgreSQL database hosted on Neon.
4. Dynamic routes render individual developer profile pages.
5. Search and filtering help visitors discover developers by relevant fields.

These describe the project architecture at a high level; consult the source code for exact data models, routes, and implementation details.

## 🚀 Running Locally

**Prerequisites:** Node.js, a package manager compatible with the repository, and access to a PostgreSQL database (such as Neon).

1. Clone the project:

   ```bash
   git clone https://github.com/p-g-udara-dilshan/Devlink-Developer-Network.git
   cd Devlink-Developer-Network
   ```

2. Install dependencies. If the repository uses npm and contains `package-lock.json`:

   ```bash
   npm install
   ```

3. Configure environment variables. Create `.env` or `.env.local` **as required by the repository** and set the database connection variable(s) referenced by the Prisma configuration. For example, **only if the project's Prisma schema uses `env("DATABASE_URL")`**:

   ```dotenv
   DATABASE_URL="your-neon-postgresql-connection-string"
   ```

   Check the actual Prisma schema and application source for the exact variable names. Never commit real credentials.

4. Apply the database setup **using the workflow configured in this repository** (for example, Prisma migrations or schema push). Do not run destructive commands against a production database.

5. Start the development server. If `package.json` provides the standard `dev` script:

   ```bash
   npm run dev
   ```

6. Open [http://localhost:3000](http://localhost:3000) (or the address printed in the terminal).

> **Setup verification:** The repository files could not be inspected when this README was prepared. Confirm the required Node.js version, package manager, environment variable names, Prisma setup command, and npm scripts against the actual source before publishing these instructions as definitive.

## 📸 Screenshots

Screenshots can help visitors evaluate the UI without signing in. To add a homepage preview, save a screenshot at `docs/images/devlink-homepage.png` and uncomment the line below:

<!-- ![DevLink developer directory homepage](docs/images/devlink-homepage.png) -->

## 🧠 What I Learned

- Structuring a full-stack application using the Next.js App Router
- Building reusable, responsive components with TypeScript and Tailwind CSS
- Creating dynamic developer profile routes and searchable directories
- Modeling and accessing persistent data with Prisma and PostgreSQL
- Integrating Next.js Server Actions with application workflows
- Deploying a database-connected web application through Vercel

## 🔐 Security & Privacy

- Store database credentials in environment variables; **never commit `.env` files or secrets**.
- Apply appropriate authorization checks to any profile-editing Server Actions.
- Validate user-supplied data on the server before writing it to the database.
- Avoid publishing real private user details in screenshots, logs, or sample data.
- Treat example developer profiles and metrics as demo content unless verified.

## 🔭 Possible Future Improvements

- More advanced developer discovery and sorting
- Improved accessibility and keyboard navigation
- Automated testing for profile and search workflows
- Additional profile customization and portfolio showcases
- Production monitoring and performance optimization

*These are potential enhancements, not claims about already-implemented features.*

## 👨‍💻 Developer

**P. G. Udara Dilshan**  
GitHub: [p-g-udara-dilshan](https://github.com/p-g-udara-dilshan)  
LinkedIn: [p-g-udara-dilshan](https://www.linkedin.com/in/p-g-udara-dilshan)  
Email: [udara.profile@gmail.com](mailto:udara.profile@gmail.com)

---

Built as a personal project to explore modern full-stack development and developer-focused user experiences.
