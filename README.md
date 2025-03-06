# Drone Management System

## Description

This project implements a **Java-based REST API** for managing drones in a medication delivery system. The system allows for drone registration, loading of medications, and monitoring the drones' state and battery levels. It is designed for a drone fleet that delivers packages (medications) to locations with difficult access.

## Functional Requirements

- **Register a drone** with specific details (serial number, model, weight limit, battery capacity, state).
- **Load a drone with medication**, ensuring the weight limit is not exceeded.
- **Check loaded medications** for a given drone.
- **Check drone availability** for loading, ensuring the battery is above 25%.
- **Check drone information**, such as battery levels.
- **Prevent drone overloading** based on its weight limit.
- **Prevent drone from entering LOADING state if battery is below 25%**.
- **Reduce battery percentage after each delivery**.

## Technologies Used

- **Java 23**
- **Spring Boot** (for creating the REST API)
- **H2 Database** (in-memory database for data storage)
- **Postman** (for testing the API endpoints)
  
## Assumptions

- Drone models are pre-defined with corresponding weight limits.
- The system will simulate battery reduction after each delivery.
- Drone states will transition based on specific conditions like loading and delivery.
  
## Setup and Installation

### Prerequisites
1. **Java 23**: Ensure you have Java 1.8 or a higher version installed. You can download it from [here](https://www.oracle.com/java/technologies/javase-jdk8-downloads.html).
2. **Maven** (or Gradle): Choose the build tool you are using.
   - To install **Maven**, follow the instructions [here](https://maven.apache.org/install.html).
   - To install **Gradle**, follow the instructions [here](https://gradle.org/install/).
3. **Postman** (optional for testing): You can download it [here](https://www.postman.com/downloads/).

### Clone the Repository

If you haven’t cloned the repository yet, you can clone it using Git:

```bash
git clone <repository-url>
cd <repository-folder>
