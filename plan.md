# Project Plan: CodeNexus API

**Description:** A collaborative code review and knowledge sharing platform API built with Rust and Actix-web. Enables users to upload code snippets, request reviews, and create a searchable knowledge base.


## Development Goals

- [ ] Set up the basic Actix Web server in src/main.rs, including database connection pooling using Diesel and r2d2, and configure CORS.
- [ ] Define database models (User, Snippet, Review) in src/models.rs using Diesel's ORM capabilities.
- [ ] Create Diesel schema definitions in src/schema.rs and generate the required migrations (users, snippets, reviews) using `diesel migration generate` and populate the up/down sql files.
- [ ] Implement user authentication (registration, login) with password hashing using bcrypt and JWT-based authentication in src/handlers.rs and corresponding routes in src/routes.rs.
- [ ] Implement CRUD operations for code snippets (create, read, update, delete) with proper authorization checks in src/handlers.rs and corresponding routes in src/routes.rs.
- [ ] Implement a review system where users can request and submit reviews for code snippets, also with proper authorization in src/handlers.rs and corresponding routes in src/routes.rs.
- [ ] Implement a search functionality for snippets based on keywords and tags using database queries in src/handlers.rs.
- [ ] Add input validation and sanitization to prevent common security vulnerabilities (e.g., SQL injection, XSS) in src/handlers.rs.
- [ ] Implement error handling and logging for debugging and monitoring purposes.
- [ ] Configure Actix-files to serve static content (e.g., documentation, frontend assets)
