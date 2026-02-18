# Java Web Application with Servlets and JSP

This project is a demonstration of a traditional Java Web application structured using the **Model-View-Controller (MVC)** architectural pattern. It highlights the lifecycle of Servlets and the usage of JavaServer Pages (JSP) for rendering views.



## Characteristics of the Project

* **Technology Stack**: Java EE / Jakarta EE.
* **Build Tool**: Maven (`pom.xml`) for managing dependencies and packaging.
* **Application Server**: Apache Tomcat (10.x or higher recommended).
* **Architecture**: MVC (Servlet as Controller, JSP as View, Java POJO as Model).
* **Servlet Mapping**: Utilizes Java Annotations (`@WebServlet`) for clean routing.

## Prerequisites

* **Java JDK**: Version 17 or higher.
* **Maven**: Installed and configured in your system path.
* **Apache Tomcat**: Installed (recommended version 10.1+ for Jakarta EE compatibility).

## Project Structure

The project follows the standard Maven directory structure for web applications:

```text
demo/
├── pom.xml                 # Maven configuration
└── src/
    └── main/
        ├── java/
        │   └── com/example/ # Backend Java code (Servlets, Models)
        └── webapp/
            ├── WEB-INF/
            │   └── web.xml # Web application descriptor
            ├── index.jsp   # Main view
            └── hello.jsp   # JSP view example
```
## How to Build and Run

### 1. Build the WAR file
Run the following command in the root of the project to compile the code and generate the `.war` package:

```bash
mvn clean package
```
## 2. Deploy to Tomcat
1. Locate the generated file `target/demo.war`.
2. Copy this file into the `webapps` directory of your Apache Tomcat installation.
3. Start Tomcat (run `bin/startup.bat` on Windows or `bin/startup.sh` on Linux/macOS).



## 3. Access the Application
Open your browser and navigate to: [http://localhost:8081/demo/hello](http://localhost:8081/demo/hello)
