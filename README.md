**Implementation cinema app**
 
Technology in project: Spring, Hibernate, JWT authentication.

Roles and first Admin user injected inside DataInitializer class using annotation @PostConstruct.<br/>
Roles: ADMIN, USER.<br/>
User:<br/>
Login - admin@i.ua<br/>
Pass - admin123

Access for the endpoint by roles:<br/>
POST: /register - all<br/>
GET: /cinema-halls - user/admin<br/>
POST: /cinema-halls - admin<br/>
GET: /movies - user/admin<br/>
POST: /movies - admin<br/>
GET: /movie-sessions/available - user/admin<br/>
POST: /movie-sessions - admin<br/>
PUT: /movie-sessions/{id} - admin<br/>
DELETE: /movie-sessions/{id} - admin<br/>
GET: /orders - user<br/>
POST: /orders/complete - user<br/>
PUT: /shopping-carts/movie-sessions - user<br/>
GET: /shopping-carts/by-user - user<br/>
GET: /users/by-email - admin<br/>