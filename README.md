# First Project — Java Spring (Vistula)

A small **educational Spring Boot project** that demonstrates:
- a simple **REST endpoint** (`/`) returning plain text,
- a **Thymeleaf page** (`/greeting`) with a request parameter,
- usage of **static resources** (image from `src/main/resources/static/images`).

---

## 🚀 What This Project Does

### 1) `GET /`
Returns a simple text response in the browser (to verify that the controller works).

Example response:
- `Hello Vistula, in my first Spring controller.`

---

### 2) `GET /greeting`
Opens an HTML page (`greeting.html`) rendered with **Thymeleaf** and displays a name.

- If `name` is not provided → default value **World** is used
- If `name` is provided → it is displayed on the page

Examples:
- `http://localhost:8080/greeting` → `Hello, World!`
- `http://localhost:8080/greeting?name=Vistula` → `Hello, Vistula!`

---

### 3) Static resources (images)
The project contains an image:

`src/main/resources/static/images/vistula.png`

This image is displayed on the `greeting.html` page.

---

## 🧩 Tech Stack

- Java
- Spring Boot
- Spring Web (Controller + GET endpoints)
- Thymeleaf (HTML templates)
- Static resources (images)

---

## 📁 Project Structure (key parts)

- `src/main/java/.../controller/HelloController.java` — controller with `/` and `/greeting` endpoints
- `src/main/resources/templates/greeting.html` — Thymeleaf HTML template
- `src/main/resources/static/images/vistula.png` — static image resource
  ![image alt](https://github.com/eternalrot/FirstProjectJavaSpring/blob/main/first.png?raw=true)

---

## ▶️ How to Run the Project

### Using IntelliJ IDEA
1. Open the project
2. Run `FirstProjectJavaSpringApplication`
3. Open in your browser:
   - `http://localhost:8080/`
   - `http://localhost:8080/greeting`
   - `http://localhost:8080/greeting?name=Vistula`

### Using Maven
```bash
mvn spring-boot:run
