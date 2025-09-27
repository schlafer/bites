## Project Overview

- Cuisines
  1. GET /cuisines
      - Retrieves all cuisines.
  2. GET /cuisines/:cuisine
      - Retrieves all restaurants for a specific cuisine.

- Restaurants
  1. GET /restaurants/search
      - Searches for restaurants by name.
      
  2. POST /restaurants 
      - Creates a new restaurant.
  
  3. GET /restaurants
      - Retrieves paginated list of restaurants sorted by rating.
  
  4. POST /restaurants/:id/reviews
      - Adds a new review for a restaurant.
  
  5. GET /restaurants/:id/reviwes
      - Retrieves paginated list of reviews for a restaurant.
  
  6. DELETE /restaurants/:restaurantId/reviews/:reviewId
      - Deletes a specific review for a restaurant.
  
  7. GET /restaurants/:restaurantId/weather
      - Retrieves weather information for a restaurant's location.
  
  8. GET /restaurants/:id
      - Retrieves details of a specific restaurant.

## Tech-stack

- Node
- Express
- node-redis (Hashes, Lists, Sets, Sorted Sets, Strings, RedisJSON, RediSearch, Bloom Filters)
- TypeScript
- Zod 

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
