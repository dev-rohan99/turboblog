# 📖 Blog Application (NestJS + Next.js)

A modern full-stack **blog application** built with **NestJS (backend)** and **Next.js (frontend)**.  
This project demonstrates real-world features like **user authentication, posts, tags, and comments**, with a clean and responsive UI.  

---

## 🚀 Features

- 🔐 **User Authentication**: Register, login, and manage profiles  
- 📝 **Posts**: Create, edit, delete, and view blog posts  
- 🏷️ **Tags**: Categorize posts and filter by tags  
- 💬 **Comments**: Add, view, and manage comments on posts  
- 🎨 **Frontend UI**: Built with Next.js, TailwindCSS, and shadcn/ui  
- 🌙 **Dark Mode**: Toggle between light and dark themes  
- ✨ **Animations**: Smooth transitions with Framer Motion  
- 🗄️ **Database Schema**: Designed with Eraser (User, Post, Tag, Comment, PostTag)  
- 📦 **Scalable Backend**: NestJS with Prisma ORM (PostgreSQL)  

---

## 🛠 Tech Stack

**Frontend**  
- [Next.js 14](https://nextjs.org/)  
- [TailwindCSS](https://tailwindcss.com/)  
- [shadcn/ui](https://ui.shadcn.com/)  
- [Framer Motion](https://www.framer.com/motion/)  

**Backend**  
- [NestJS](https://nestjs.com/)  
- [Prisma](https://www.prisma.io/) ORM  
- [PostgreSQL](https://www.postgresql.org/) (can be swapped with MongoDB)  

**Other Tools**  
- [Eraser](https://eraser.io/) for ERD/schema design  
- [Vercel](https://vercel.com/) for frontend deployment  
- Node.js server / Docker for backend deployment  

---

## 📂 Project Structure

/blog-app
│── /frontend # Next.js app (UI)
│── /backend # NestJS app (API)
│── /prisma # Prisma schema and migrations
│── README.md # Project documentation


---

## ⚡ Installation & Setup

### 1️⃣ Clone the Repository
```bash
git clone https://github.com/your-username/blog-app.git
cd blog-app

2️⃣ Setup Frontend
cd frontend
npm install
npm run dev


Runs the Next.js app at: http://localhost:3000

3️⃣ Setup Backend
cd backend
npm install
npm run start:dev


Runs the NestJS app at: http://localhost:5000

4️⃣ Configure Database (Prisma + PostgreSQL)
cd backend
npx prisma migrate dev --name init
npx prisma generate

🔑 Mock Data

The frontend currently uses mock JSON arrays for:

Users

Posts

Tags

Comments

This allows you to test the UI before connecting the backend API.

📜 API Endpoints (Planned)
Method	Endpoint	Description
POST	/auth/register	Register a new user
POST	/auth/login	Login user
GET	/users/:id	Get user profile
PUT	/users/:id	Update user profile
GET	/posts	Get all posts
GET	/posts/:id	Get single post
POST	/posts	Create new post
PUT	/posts/:id	Update post
DELETE	/posts/:id	Delete post
GET	/tags	Get all tags
POST	/tags	Create new tag
GET	/posts/:id/comments	Get comments for a post
POST	/posts/:id/comments	Add comment to a post
🗺 Database Schema (ERD)

Entities:

User

Post

Tag

Comment

PostTag (many-to-many join table)

Designed with Eraser.

📸 Screenshots (to add later)

Home page with posts

Single post with comments

Auth pages (login/register)

Profile page

🎯 Purpose

This project is built for learning NestJS with real-world implementation, while practicing clean UI development in Next.js.
It covers the end-to-end workflow:

Database schema design

Backend API development (NestJS + Prisma)

Frontend integration (Next.js + TailwindCSS + shadcn/ui)

🤝 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you’d like to change.

📄 License

This project is licensed under the MIT License.


---

This README is **professional, structured, and beginner-friendly** — perfect for GitHub.  

👉 Do you also want me to create a **`mock-data.js` file** (users, posts, comments, tags) so you can include it in