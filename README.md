# ☕ Maven Project

> A Java application built using **Apache Maven** to demonstrate build automation, dependency management, project configuration, unit testing, and DevOps integration.

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk)
![Maven](https://img.shields.io/badge/Apache-Maven-C71A36?style=for-the-badge&logo=apachemaven)
![JUnit](https://img.shields.io/badge/JUnit-5-25A162?style=for-the-badge&logo=junit5)
![Git](https://img.shields.io/badge/Git-Version_Control-F05032?style=for-the-badge&logo=git)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)

---

# 📖 About the Project

This project was developed to learn the fundamentals of **Apache Maven**, a powerful build automation and dependency management tool for Java applications.

The project demonstrates how Maven simplifies Java development by managing dependencies, automating builds, executing unit tests, and packaging applications into deployable artifacts.

It also serves as the **foundation for future DevOps practices**, including Gradle, Jenkins, Ansible, CI/CD Pipelines, and Azure DevOps.

---

# 🎯 Objectives

- Create a Maven Project
- Understand Maven Directory Structure
- Configure `pom.xml`
- Manage Project Dependencies
- Configure Maven Plugins
- Execute Maven Build Lifecycle
- Perform Unit Testing
- Package Java Applications
- Prepare the project for DevOps workflows

---

# ✨ Features

- Standard Maven Project Structure
- Java Application Development
- Dependency Management
- Build Automation
- Plugin Configuration
- JUnit Testing
- JAR Packaging
- Easy Project Maintenance
- Git & GitHub Integration

---

# 🛠 Technologies Used

| Technology | Purpose |
|------------|---------|
| Java 21 | Programming Language |
| Apache Maven | Build Automation Tool |
| Maven Wrapper | Portable Maven Execution |
| JUnit 5 | Unit Testing |
| Git | Version Control |
| GitHub | Source Code Hosting |
| Command Prompt (CMD) | Running Maven Commands |

---

# 📂 Project Structure

```text
maven-project/
│
├── .mvn/
├── gradle/
├── src/
│   ├── main/
│   │   └── java/
│   └── test/
│       └── java/
├── target/
├── pom.xml
├── build.gradle
├── settings.gradle
├── gradlew
├── gradlew.bat
├── README.md
└── .gitignore
```

---

# ⚙ Software Requirements

Before running the project, install:

- Java Development Kit (JDK 21)
- Apache Maven
- Git
- GitHub Account
- Java IDE (IntelliJ IDEA / Eclipse / VS Code)

---

# 🚀 Installation Guide

## Step 1 — Install Java

Download and install **Java Development Kit (JDK 21)**.

Verify installation:

```bash
java -version
```

---

## Step 2 — Install Apache Maven

Download Apache Maven and configure:

- `JAVA_HOME`
- `MAVEN_HOME`
- Add Maven's **bin** folder to the System PATH

Verify installation:

```bash
mvn -version
```

---

## Step 3 — Clone Repository

```bash
git clone https://github.com/isra-is/maven-project.git
```

---

## Step 4 — Navigate into Project

```bash
cd maven-project
```

---

# ▶ Running the Project

### Compile

```bash
mvn compile
```

### Run Tests

```bash
mvn test
```

### Package

```bash
mvn package
```

### Install

```bash
mvn install
```

### Clean

```bash
mvn clean
```

---

# 📦 Maven Build Lifecycle

| Phase | Description |
|--------|-------------|
| validate | Validates project structure |
| compile | Compiles Java source code |
| test | Executes unit tests |
| package | Creates a JAR file |
| install | Installs package into local repository |
| deploy | Deploys package to remote repository |

---

# 📄 Understanding pom.xml

The **Project Object Model (POM)** is the heart of every Maven project.

It contains:

- Project Information
- Dependencies
- Plugins
- Build Configuration
- Version Details
- Packaging Information

---

# 📚 Learning Outcomes

After completing this project, I learned:

- Java Project Development using Maven
- Installing and Configuring Java
- Installing and Configuring Maven
- Maven Directory Structure
- Working with `pom.xml`
- Managing Dependencies
- Configuring Plugins
- Running Maven Lifecycle Commands
- Writing Unit Tests
- Packaging Java Applications
- Uploading Projects to GitHub

---

# 🚀 Future Scope

This project acts as the starting point for advanced DevOps concepts.

It can be integrated with:

- ✅ Gradle Build Tool
- ✅ Jenkins Automation Server
- ✅ Continuous Integration (CI)
- ✅ Continuous Deployment (CD)
- ✅ Ansible Configuration Management
- ✅ Azure DevOps Pipelines
- ✅ Azure App Services
- ✅ GitHub Actions

---

# 🔄 DevOps Workflow

```text
Java Source Code
        │
        ▼
Apache Maven
        │
        ▼
Compile & Test
        │
        ▼
Generate JAR
        │
        ▼
GitHub Repository
        │
        ▼
Jenkins CI Pipeline
        │
        ▼
Ansible Deployment
        │
        ▼
Azure DevOps Pipeline
        │
        ▼
Application Deployment
```

---

# 📸 Output

Add screenshots here:

- Java Program Output
- Maven Build Output
- JUnit Test Result
- Generated JAR File
- Project Structure
- GitHub Repository

Example:

```
images/
├── project-structure.png
├── compile-output.png
├── test-output.png
├── package-output.png
└── github-repository.png
```

---

# 🤝 Contributing

Contributions, improvements, and suggestions are always welcome.

1. Fork the repository
2. Create a new branch
3. Commit your changes
4. Push to GitHub
5. Open a Pull Request

---

# 👩‍💻 Author

**Isra Zainab**

**B.E. Computer Science & Engineering**  
*(IoT, Cybersecurity & Blockchain Technology)*

🔗 GitHub: https://github.com/isra-is

---

# 📜 License

This project is created for educational and learning purposes.

---

⭐ If you found this repository useful, consider giving it a Star!
