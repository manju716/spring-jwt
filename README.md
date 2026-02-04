
```
spring-jwt
│
├── .idea/                  # IntelliJ IDEA config (ignored in Git)
├── .mvn/                   # Maven wrapper files
│
├── src
│   ├── main
│   │   ├── java
│   │   │   └── com.example.jwt
│   │   │       ├── SpringJwtApplication.java
│   │   │       │
│   │   │       ├── config
│   │   │       │   ├── SecurityConfig.java
│   │   │       │   └── JwtFilter.java
│   │   │       │
│   │   │       ├── controller
│   │   │       │   ├── AuthController.java
│   │   │       │   └── TestController.java
│   │   │       │
│   │   │       ├── model
│   │   │       │   └── User.java
│   │   │       │
│   │   │       ├── repository
│   │   │       │   └── UserRepository.java
│   │   │       │
│   │   │       └── service
│   │   │           ├── JwtService.java
│   │   │           └── UserService.java
│   │   │
│   │   └── resources
│   │       └── application.properties
│   │
│   └── test
│       └── java
│
├── target/                 # Build output (ignored in Git)
├── .gitignore
└── pom.xml
```

output
POST http://localhost:8080/auth/register
POST http://localhost:8080/auth/login
eyJhbGciOiJIUzI1NiJ9.eyJzdWIiOiJtYW5qdWxhIiwiaWF0IjoxNzAwMDAwMDAwLCJleHAiOjE3MDAwMDM2MDB9...(token)
GET http://localhost:8080/test/hello
output
```
