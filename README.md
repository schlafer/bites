## Tech Used

- Node
- Express
- Redis (Hashes, Lists, Sets, Sorted Sets & Strings)
- TypeScript
- Zod validation (& Express middleware)
- RedisJSON
- Redis Search
- Redis Bloom Filters

## Usage
To use this project, you will first need to have a running Redis Stack instance. View the [Redis](https://redis.io/docs/latest/operate/oss_and_stack/install/) guide to get this set-up on your environment

### Development

1. Clone the repo
2. Run ```pnpm install```
3. Run ```pnpm run dev```

### Production

1. Clone the repo
2. Run ```pnpm install```
3. Run ```pnpm run build```
4. Run ```pnpm run start```

## Scope

Future features and improvements:

- Authentication and Authorization

  - Implement JWT-based user authentication, including registration and login routes.
  - Introduce Role-Based Access Control (RBAC) to restrict access to certain routes based on user roles (e.g., admin, user).

- Advanced Redis Features

  - Utilize Redis Pub/Sub for real-time updates, enabling live communication such as updates to restaurant data or reviews.
  - Explore Redis Streams for event sourcing to record all changes as events.

- Improved Caching Strategies

    - Implement cache invalidation by setting appropriate expiration times and automatically updating the cache when underlying data changes.

- Real-Time Features with WebSockets

  - Integrate Socket.IO to add real-time functionalities like live chat, notifications, or live updates of reviews.
