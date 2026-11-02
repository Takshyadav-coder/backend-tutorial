# Backend Tutorial

A small Express and MongoDB API for users and posts.

## Requirements

- Node.js 20.19 or newer
- MongoDB running locally, or a MongoDB Atlas connection string

## Setup

1. Install dependencies:

   ```sh
   npm install
   ```

2. Create a root `.env` file from the example:

   ```sh
   cp .env.example .env
   ```

   On Windows PowerShell, use `Copy-Item .env.example .env` instead. Set `MONGODB_URI` in `.env` to your local MongoDB URL or Atlas connection string. Keep `.env` private; it is ignored by Git.

3. Start the API:

   ```sh
   npm run dev
   ```

   For a regular start, use `npm start`. The API listens on port `8000` by default; set `PORT` in `.env` to change it.

## API routes

- `POST /api/v1/users/register`
- `POST /api/v1/users/login`
- `POST /api/v1/users/logout`
- `POST /api/v1/posts/create`
- `GET /api/v1/posts/getposts`
- `PATCH /api/v1/posts/updatepost/:id`
- `DELETE /api/v1/posts/deletepost/:id`
