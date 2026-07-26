# ☕ Maven Project

<div align="center">

# Apache Maven Project

*A Java project demonstrating Maven fundamentals, build automation, dependency management, plugins, unit testing, and project packaging.*

![Java](https://img.shields.io/badge/Java-21-orange?style=for-the-badge&logo=openjdk)
![Apache Maven](https://img.shields.io/badge/Apache-Maven-C71A36?style=for-the-badge&logo=apachemaven)
![JUnit](https://img.shields.io/badge/JUnit-5-25A162?style=for-the-badge&logo=junit5)
![Git](https://img.shields.io/badge/Git-Version_Control-F05032?style=for-the-badge&logo=git)
![GitHub](https://img.shields.io/badge/GitHub-Repository-181717?style=for-the-badge&logo=github)
![License](https://img.shields.io/badge/License-Educational-blue?style=for-the-badge)

</div>

---

# 📖 Overview

This repository contains the implementation of the **Apache Maven laboratory exercise** completed as part of the **6th Semester DevOps Laboratory**.

The project demonstrates the fundamentals of Maven, including project creation, dependency management, plugin configuration, build automation, testing, packaging, and version control using Git and GitHub.

The implementation follows the objectives of the laboratory exercise while providing a practical understanding of how Maven simplifies Java application development.

---

# 🎓 Laboratory Information

| Item | Details |
|------|---------|
| Course | DevOps Laboratory |
| Semester | 6th Semester |
| Experiment | Working with Maven |
| Build Tool | Apache Maven |
| Programming Language | Java 21 |
| Testing Framework | JUnit 5 |
| Version Control | Git |
| Repository Hosting | GitHub |

---

# 📚 Table of Contents

- Overview
- Laboratory Information
- Objectives
- Technologies Used
- Software Requirements
- Java Installation
- Maven Installation
- Maven Project Structure
- Understanding `pom.xml`
- Maven Build Lifecycle
- Maven Commands
- Dependency Management
- Maven Plugins
- Unit Testing
- Building the Project
- Running the Application
- Git & GitHub Workflow
- Project Screenshots
- Learning Outcomes
- Related DevOps Topics
- Repository Purpose
- Acknowledgement
- License

---

# 🎯 Objectives

The primary objectives of this laboratory exercise are:

- Create a Maven project
- Understand Maven architecture
- Learn the standard Maven directory structure
- Configure the `pom.xml` file
- Manage project dependencies
- Configure Maven plugins
- Execute Maven build lifecycle phases
- Perform unit testing using JUnit
- Generate executable JAR files
- Understand Maven's role in DevOps
- Maintain source code using Git and GitHub

# 🛠 Technologies Used

| Technology | Version | Purpose |
|------------|---------|---------|
| Java | 21 | Programming Language |
| Apache Maven | Latest Stable Release | Build Automation & Dependency Management |
| Maven Wrapper | Included | Project-specific Maven Execution |
| JUnit | 5 | Unit Testing Framework |
| Git | Latest | Version Control |
| GitHub | - | Repository Hosting |
| Command Prompt (CMD) | Windows | Running Maven Commands |

---

# 💻 Software Requirements

Before running this project, ensure the following software is installed:

- Java Development Kit (JDK 21)
- Apache Maven
- Git
- Internet connection (for downloading Maven dependencies)
- A Java IDE (Optional)
  - IntelliJ IDEA
  - Eclipse IDE
  - Visual Studio Code

---

# ☕ Java Installation

## Step 1: Download Java

Download the latest **Java Development Kit (JDK 21)** from the official Oracle website or any compatible OpenJDK distribution.

---

## Step 2: Install Java

Run the installer and complete the installation by following the setup instructions.

---

## Step 3: Configure JAVA_HOME

Set the `JAVA_HOME` environment variable to the JDK installation directory.

Example:

```text
C:\Program Files\Java\jdk-21
```

Add the following to the system **Path**:

```text
%JAVA_HOME%\bin
```

---

## Step 4: Verify Installation

Open Command Prompt and execute:

```bash
java -version
```

Expected Output:

```text
java version "21"
```

---

# 📦 Apache Maven Installation

## Step 1: Download Maven

Download the latest stable version of **Apache Maven** from the official Apache Maven website.

---

## Step 2: Extract Maven

Extract the downloaded archive to a preferred location.

Example:

```text
C:\Program Files\Apache\Maven
```

---

## Step 3: Configure Environment Variables

Create a new environment variable:

```text
MAVEN_HOME
```

Set its value to the Maven installation directory.

Example:

```text
C:\Program Files\Apache\Maven
```

---

## Step 4: Update System PATH

Add the following to the system Path:

```text
%MAVEN_HOME%\bin
```

---

## Step 5: Verify Maven Installation

Open Command Prompt and run:

```bash
mvn -version
```

Example Output:

```text
Apache Maven 3.x.x
Java version: 21
```

---

# 📁 Creating a Maven Project

A Maven project can be created using the Maven Archetype command.

Example:

```bash
mvn archetype:generate
```

After creation, Maven automatically generates the standard project structure containing:

- Source Code
- Test Code
- `pom.xml`
- Build Configuration

---

# 📂 Standard Maven Directory Structure

```text
project-name/
│
├── src/
│   ├── main/
│   │   ├── java/
│   │   └── resources/
│   │
│   └── test/
│       ├── java/
│       └── resources/
│
├── target/
├── pom.xml
├── mvnw
├── mvnw.cmd
└── README.md
```

---

# 📌 Why Maven?

Apache Maven helps developers by:

- Managing project dependencies automatically
- Standardizing project structure
- Automating project builds
- Running unit tests
- Packaging applications
- Simplifying project maintenance
- Supporting Continuous Integration (CI) workflows

---

# ✅ Verify Everything is Ready

Run the following commands to verify the setup:

```bash
java -version
```

```bash
mvn -version
```

```bash
git --version
```

If all commands execute successfully, the development environment is ready for building and running Maven projects.
