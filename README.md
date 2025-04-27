# 🚀 DeployProject

A simple **Spring Boot** application created for testing, learning, and deployment purposes.  
Deployed live using **Render.com**.

## 🌍 Live Website
🔗 [Visit Now](https://deployproject-lg6e.onrender.com/)

## 📚 Features
- Simple Root Controller to render a static page
- Dockerfile for easy containerization
- Maven-based project structure
- Deployed on Render.com for free hosting

## 🛠 Built With
- Java 17
- Spring Boot 
- Maven
- Docker
- Thymeleaf (for rendering HTML)
- Render.com (for deployment)

## 📂 Project Structure
```
deployproject/
├── src/
│   ├── main/
│   │   ├── java/
│   │   │   └── com/example/firstproject/controller/RootController.java
│   │   ├── resources/
│   │   │   ├── static/
│   │   │   ├── templates/
│   │   │   │   └── render.html
│   │   │   └── application.properties
├── Dockerfile
├── pom.xml
└── README.md
```

## ▶️ How to Run Locally

1. **Clone the repository**
   ```bash
   git clone https://github.com/Didar1313/deployproject.git
   ```

2. **Navigate to the project directory**
   ```bash
   cd deployproject
   ```

3. **Build and Run the project**
   ```bash
   ./mvnw spring-boot:run
   ```
   or (if you have Maven installed)
   ```bash
   mvn spring-boot:run
   ```

4. **Access the application**
   ```
   http://localhost:8080/
   ```

## ✨ Controller Overview

```java
@Controller
public class RootController {

    @GetMapping("/")
    public String wellComePage() {
        return "render"; // This loads render.html from templates
    }
}
```
⚡ **Note**: Make sure you have a `render.html` page inside `src/main/resources/templates/`.

## 📦 Deployment
- Docker is used for creating the container.
- Application is deployed on Render.com with automatic build from GitHub.


