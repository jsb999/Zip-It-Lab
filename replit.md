# Zip It (Java)

## Overview
This is a Java console application project built with Gradle. It's designed as a programming lab assignment for implementing a compression/zip utility. The project uses Java 21 with Gradle 8.10.2 as the build system.

## Recent Changes
- **2024-12-02**: Initial Replit environment setup completed
  - Configured Gradle build system
  - Set up workflow to run the application
  - Verified Java toolchain configuration

## Project Architecture

### Technology Stack
- **Language**: Java 21 (using Gradle's automatic toolchain provisioning)
- **Build System**: Gradle 8.10.2 with Gradle Wrapper
- **Testing Framework**: JUnit Jupiter 5.10.3
- **Dependencies**: Google Guava 33.2.1-jre

### Project Structure
```
zip-it-java-template/
├── app/
│   ├── src/
│   │   ├── main/java/org/example/
│   │   │   └── App.java          # Main application entry point
│   │   └── test/java/org/example/
│   │       └── AppTest.java       # Unit tests
│   └── build.gradle               # Application build configuration
├── gradle/                        # Gradle wrapper and version catalog
├── settings.gradle                # Project settings
├── gradlew                        # Gradle wrapper script (Unix)
└── gradlew.bat                    # Gradle wrapper script (Windows)
```

### Key Configuration
- **Main Class**: `org.example.App`
- **Standard Input**: Configured to accept console input via `standardInput = System.in`
- **Java Toolchain**: Automatically provisions Java 21 even though system Java is 19

## Development

### Building the Project
```bash
./gradlew build
```

### Running Tests
```bash
./gradlew test
```

### Running the Application
The application runs automatically via the "Run Application" workflow, or manually:
```bash
./gradlew run --quiet --console=plain
```

The `--quiet` and `--console=plain` flags reduce Gradle's verbose output.

## Workflow Configuration
- **Name**: Run Application
- **Command**: `./gradlew run --quiet --console=plain`
- **Output Type**: Console (interactive command-line application)

## Notes
- This is a console/terminal-based application with no frontend or backend server components
- The project uses Gradle's Java toolchain feature to automatically download and use Java 21
- The application is configured to accept standard input for interactive user interaction
- Lab instructions available at: https://morethanequations.com/Computer-Science/Labs/Zip-It
