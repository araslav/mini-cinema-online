**Implementation cinema app**
 
Technology in project: Spring, Hibernate, JWT authentication.

Roles and first Admin user injected inside DataInitializer class using annotation @PostConstruct.
Roles: ADMIN, USER.
User:
Login - admin@i.ua
Pass - admin123

Access for the endpoint by roles:
POST: /register - all
GET: /cinema-halls - user/admin
POST: /cinema-halls - admin
GET: /movies - user/admin
POST: /movies - admin
GET: /movie-sessions/available - user/admin
POST: /movie-sessions - admin
PUT: /movie-sessions/{id} - admin
DELETE: /movie-sessions/{id} - admin
GET: /orders - user
POST: /orders/complete - user
PUT: /shopping-carts/movie-sessions - user
GET: /shopping-carts/by-user - user
GET: /users/by-email - admin