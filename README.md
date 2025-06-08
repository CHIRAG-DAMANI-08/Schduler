# 🚀 CodeAtlas

A modern, full-stack scheduling and event booking platform built with Next.js, Prisma, Clerk, and Google Calendar integration. Effortlessly manage your availability, host events, and let others book meetings with you—complete with automatic Google Meet links! 🌐📅

---

## ✨ Features

- **User Authentication**: Secure sign-up and login with Clerk.
- **Profile & Username Management**: Unique usernames, profile images, and user details.
- **Event Scheduling**: Create, update, and delete events with customizable durations and privacy settings.
- **Availability Management**: Set your weekly availability and minimum time gaps between bookings.
- **Booking System**: Attendees can book public events, automatically generating Google Calendar events and Meet links.
- **Google Calendar Integration**: OAuth2-based, with automatic event creation and video conferencing.
- **Dashboard**: See your upcoming meetings and latest updates at a glance.

---

## 🛠️ Tech Stack

- **Frontend**: Next.js (App Router)
- **Backend**: Node.js, Prisma ORM
- **Database**: PostgreSQL
- **Authentication**: Clerk
- **Calendar Integration**: Google Calendar API
- **UI**: (Add your UI library here, e.g., Tailwind CSS, Chakra UI)

---

## 📦 Project Structure

```
├── actions/           # Server actions for users, events, bookings, etc.
├── app/               # Next.js app directory
├── prisma/            # Prisma schema and migrations
├── lib/               # Utility functions (e.g., checkUser)
```

---

## 🚦 Getting Started

1. **Clone the repo:**
   ```bash
   git clone https://github.com/yourusername/codeatlas.git
   cd codeatlas
   ```
2. **Install dependencies:**
   ```bash
   npm install
   ```
3. **Set up environment variables:**
   - `DATABASE_URL` for PostgreSQL
   - Clerk and Google OAuth credentials (see `.env.example`)
4. **Run migrations:**
   ```bash
   npx prisma migrate deploy
   ```
5. **Start the dev server:**
   ```bash
   npm run dev
   ```

---

## 🔑 Environment Variables

- `DATABASE_URL` – PostgreSQL connection string
- `CLERK_SECRET_KEY`, `CLERK_PUBLISHABLE_KEY` – Clerk credentials
- `GOOGLE_CLIENT_ID`, `GOOGLE_CLIENT_SECRET` – Google OAuth credentials

---

## 📚 Key Files

- `actions/users.js` – User profile and username logic
- `actions/events.js` – Event CRUD and details
- `actions/bookings.js` – Booking creation and Google Calendar integration
- `actions/availability.js` – User availability management
- `lib/checkUser.js` – Ensures Clerk users exist in your DB
- `prisma/schema.prisma` – Database schema

---

## 📝 License

MIT

---

## 🙌 Contributing

Pull requests are welcome! For major changes, please open an issue first to discuss what you would like to change.

---

## 📣 Acknowledgements

- [Next.js](https://nextjs.org/)
- [Prisma](https://www.prisma.io/)
- [Clerk](https://clerk.com/)
- [Google Calendar API](https://developers.google.com/calendar)

---

> Built with ❤️ for seamless scheduling and collaboration!

        
