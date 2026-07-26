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

# 📄 Understanding `pom.xml`

The **Project Object Model (POM)** is the central configuration file of every Maven project.

The `pom.xml` file contains all the information required to build and manage the project, including project details, dependencies, plugins, and build configurations.

Typical information stored in the POM includes:

- Project Name
- Group ID
- Artifact ID
- Version
- Packaging Type
- Dependencies
- Build Plugins
- Project Properties

Example:

```xml
<project>
    <modelVersion>4.0.0</modelVersion>

    <groupId>com.example</groupId>
    <artifactId>maven-project</artifactId>
    <version>1.0-SNAPSHOT</version>

</project>
```

---

# 📦 Dependency Management

One of Maven's key features is **automatic dependency management**.

Instead of manually downloading external libraries, dependencies are declared in the `pom.xml` file. Maven automatically downloads them from the configured repositories.

Example:

```xml
<dependencies>

    <dependency>
        <groupId>org.junit.jupiter</groupId>
        <artifactId>junit-jupiter</artifactId>
        <version>5.10.0</version>
        <scope>test</scope>
    </dependency>

</dependencies>
```

Benefits include:

- Automatic dependency downloads
- Version management
- Reduced manual work
- Easier project maintenance

---

# 🔌 Maven Plugins

Plugins extend Maven's functionality and automate common development tasks.

Some commonly used plugins include:

| Plugin | Purpose |
|---------|---------|
| Maven Compiler Plugin | Compiles Java source code |
| Maven Surefire Plugin | Executes unit tests |
| Maven JAR Plugin | Creates executable JAR files |
| Maven Clean Plugin | Removes previous build files |

Plugins are configured within the `pom.xml` file.

---

# 🔄 Maven Build Lifecycle

Maven organizes the build process into a sequence of lifecycle phases.

The default lifecycle consists of:

| Phase | Description |
|--------|-------------|
| Validate | Checks project structure and configuration |
| Compile | Compiles source code |
| Test | Executes unit tests |
| Package | Creates a distributable package (JAR) |
| Verify | Performs additional quality checks |
| Install | Installs the package into the local repository |
| Deploy | Publishes the package to a remote repository |

Each phase automatically executes all previous phases.

Example:

Running

```bash
mvn package
```

will execute:

- Validate
- Compile
- Test
- Package

---

# ⚙️ Common Maven Commands

| Command | Description |
|----------|-------------|
| `mvn clean` | Deletes previously generated build files |
| `mvn compile` | Compiles the project |
| `mvn test` | Runs unit tests |
| `mvn package` | Creates a JAR package |
| `mvn install` | Installs the package into the local repository |
| `mvn verify` | Performs project verification |
| `mvn deploy` | Deploys the package to a remote repository |

---

# 📁 Maven Repository

Maven stores downloaded libraries in the **Local Repository**.

Default location:

```text
C:\Users\<username>\.m2\repository
```

If a dependency is not available locally, Maven downloads it automatically from a remote repository.

---

# 🌐 Maven Central Repository

The **Maven Central Repository** is the default online repository used by Maven.

It contains thousands of open-source Java libraries and plugins that can be added to projects simply by declaring them in the `pom.xml` file.

---

# 🧪 Unit Testing

Unit testing ensures that individual components of the application function correctly.

This project uses **JUnit 5** for testing.

Run tests using:

```bash
mvn test
```

Successful execution confirms that the implemented test cases have passed.

---

# 💡 Advantages of Maven

- Standardized project structure
- Automated dependency management
- Build automation
- Simplified project maintenance
- Easy integration with IDEs
- Supports Continuous Integration (CI)
- Plugin-based architecture
- Improved project portability

---

# 📚 Key Concepts Learned

Through this laboratory exercise, the following concepts were explored:

- Apache Maven
- Maven Project Structure
- Project Object Model (POM)
- Dependency Management
- Maven Plugins
- Maven Lifecycle
- Build Automation
- Unit Testing
- Packaging Java Applications
- Repository Management

# 🚀 Building and Running the Project

Once Java and Maven are installed successfully, the project can be built and executed using Maven commands.

### Compile the Project

```bash
mvn compile
```

Compiles all source files located in the `src/main/java` directory.

---

### Execute Unit Tests

```bash
mvn test
```

Runs all test cases present in the `src/test/java` directory.

---

### Package the Project

```bash
mvn package
```

Compiles the project, runs tests, and generates a JAR file inside the `target` directory.

---

### Install the Project

```bash
mvn install
```

Builds the project and installs the generated artifact into the local Maven repository for reuse in other Maven projects.

---

### Clean the Project

```bash
mvn clean
```

Removes all previously generated build files from the `target` directory.

---

# 📂 Build Output

After a successful build, Maven generates the following output:

```text
target/
│
├── classes/
├── generated-sources/
├── generated-test-sources/
├── maven-status/
├── surefire-reports/
├── test-classes/
└── *.jar
```

The generated JAR file can be found inside the **target/** directory.

---

# 🌐 Version Control with Git

Git is used to track project changes and maintain version history.

### Initialize Git

```bash
git init
```

### Check Repository Status

```bash
git status
```

### Add Files

```bash
git add .
```

### Commit Changes

```bash
git commit -m "Initial Maven project"
```

---

# ☁️ Uploading to GitHub

Create a repository on GitHub and connect it with the local project.

```bash
git remote add origin https://github.com/your-username/your-repository.git
```

Push the project:

```bash
git branch -M main
git push -u origin main
```

Once uploaded, the repository can be accessed and managed through GitHub.

---

# 📸 Screenshots

You may include screenshots such as:

- Project Folder Structure
- `pom.xml`
- Java Program Output
- `mvn compile`
- `mvn test`
- `mvn package`
- Generated JAR File
- GitHub Repository

Example:

```text
images/
│
├── project-structure.png
├── pom-file.png
├── compile-output.png
├── test-output.png
├── package-output.png
├── generated-jar.png
└── github-repository.png
```

---

# 🎓 Learning Outcomes

After completing this laboratory exercise, the following concepts were understood:

- Apache Maven fundamentals
- Java project management
- Maven directory structure
- Project Object Model (POM)
- Dependency management
- Maven plugins
- Maven build lifecycle
- Unit testing with JUnit
- Build automation
- Packaging Java applications
- Git version control
- GitHub repository management

---

# 🔄 Related DevOps Concepts

The concepts learned in this experiment provide a foundation for advanced DevOps tools and practices, including:

- Gradle
- Jenkins
- Continuous Integration (CI)
- Continuous Deployment (CD)
- Ansible
- Azure DevOps
- GitHub Actions
- Build and Release Pipelines

---

# 📖 References

- Apache Maven Documentation
- Oracle Java Documentation
- Git Documentation
- GitHub Documentation

---

# 📌 Repository Purpose

This repository is maintained as a record of the practical implementation completed during the **6th Semester DevOps Laboratory**.

It demonstrates the application of Apache Maven concepts for educational purposes and serves as a reference for learning Java project management and build automation.

---

# 📚 Acknowledgement

This repository contains the practical implementation of a laboratory exercise completed as part of the **6th Semester DevOps Laboratory**.

The experiment objectives and concepts are based on the laboratory curriculum provided by the institution. This repository is intended solely for educational and learning purposes.

---

# 📜 License

This repository is intended for **educational and academic purposes only**.

The implementation and documentation in this repository are shared to support learning and practice.
