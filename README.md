# AI Companion with Next.js 13, React, Tailwind, Prisma, Stripe

![Image of project](https://user-images.githubusercontent.com/23248726/257111735-ef2913b1-eafe-4829-9018-f2ca5a7ba651.png)

A powerful AI companion application built using Next.js 13, React, Tailwind CSS, Prisma, and Stripe.

---

## Features

- Tailwind design
- Tailwind animations and effects
- Full responsiveness
- Clerk Authentication (Email, Google, 9+ Social Logins)
- Client form validation and handling using react-hook-form
- Server error handling using react-toast
- Image Generation Tool (Open AI)
- Video Generation Tool (Replicate AI)
- Conversation Generation Tool (Open AI)
- Music Generation Tool (Replicate AI)
- Page loading state
- Stripe monthly subscription
- Free tier with API limiting
- How to write POST, DELETE, and GET routes in route handlers (app/api)
- How to fetch data in server react components by directly accessing the database (WITHOUT API! like Magic!)
- How to handle relations between Server and Child components!
- How to reuse layouts
- Folder structure in Next 13 App Router

---

## Prerequisites

Node version 18.x.x

---

**Cloning the repository**

```bash
git clone https://github.com/AntonioErdeljac/next13-ai-companion.git
```

**Install packages**
```bash
npm i
```

## Setup .env file
```
NEXT_PUBLIC_CLERK_PUBLISHABLE_KEY=
CLERK_SECRET_KEY=

NEXT_PUBLIC_CLERK_SIGN_IN_URL=/sign-in
NEXT_PUBLIC_CLERK_SIGN_UP_URL=/sign-up
NEXT_PUBLIC_CLERK_AFTER_SIGN_IN_URL=/dashboard
NEXT_PUBLIC_CLERK_AFTER_SIGN_UP_URL=/dashboard

OPENAI_API_KEY=
REPLICATE_API_TOKEN=

PINECONE_API_KEY=
PINECONE_ENVIRONMENT=
PINECONE_INDEX=

UPSTASH_REDIS_REST_URL=
UPSTASH_REDIS_REST_TOKEN=

NEXT_PUBLIC_CLOUDINARY_CLOUD_NAME=

DATABASE_URL=

STRIPE_API_KEY=
STRIPE_WEBHOOK_SECRET=

NEXT_PUBLIC_APP_URL="http://localhost:3000"
```

# Setup Prisma

**Add MySQL Database (I used PlanetScale)**
```
npx prisma db push
```
**Seed categories:**

```
node scripts/seed.ts
```
 **Start the app**

```
npm run dev
```
## Available commands

Running commands with npm: `npm run [command]`

| Command | Description |
|---------|-------------|
| `dev`     | Starts a development instance of the app |
