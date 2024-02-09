# Polls

This is a polling application built with TypeScript, Fastify, Prisma, and Redis.

## Prerequisites

- Node.js
- Docker and Docker Compose

## Getting Started

1. Clone the repository:

```sh
git clone https://github.com/lucasali/polls-api.git
cd polls-api
```

2. Install the dependencies:

```sh
pnpm install
```

3. Start the PostgreSQL and Redis services using Docker Compose:

```sh
docker-compose up -d
```

4. Run the development server:

```sh
npm run dev
```

The server will start on http://localhost:3333.

## Project Structure

- src/http/server.ts: The main server file where Fastify is configured and routes are registered.
- src/http/routes/: Contains the route handlers for creating polls, getting polls, and voting on polls.
- src/http/ws/poll-results.ts: Handles WebSocket connections for real-time poll results.
- src/utils/voting-pub-sub.ts: Handles the publishing and subscribing of vote updates using Redis.

## Contributing

Contributions are welcome! Please read our contributing guide to learn about our development process, how to propose bugfixes and improvements, and how to build and test your changes.

## License

This project is licensed under the ISC License - see the LICENSE file for details.
