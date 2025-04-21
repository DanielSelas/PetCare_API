# PetCare API – Backend for PetCare SDK

**PetCare API** is the backend service for the PetCare SDK, developed as part of a seminar project. It provides a RESTful interface for managing pet-related data such as pet profiles, health info, and interactions with other app modules like PetCareLib and the mobile app frontend.

Repository: [DanielSelas/PetCare_API](https://github.com/DanielSelas/PetCare_API)

---

## Overview

The API serves as the foundation of the PetCare ecosystem, allowing developers to store, retrieve, and manage pet data in a structured and secure way. It is built to be lightweight, extendable, and easy to integrate with Android applications via the companion PetCareLib library.

---

## Core Features

### Pet Management
- Add, edit, or delete pet profiles
- Track details like breed, age, weight, gender, and vaccination status

### Owner Integration
- Associate pets with specific owners
- View owner details and manage pet ownership

### Smart Structuring
- Designed to support future enhancements such as reminders, medical history, or nutrition tracking

### Lightweight Security
- Basic validation and input sanitization
- Easily extendable to include user authentication

---

## Tech Stack

- Backend Framework: Spring Boot (Java)
- Database: In-memory or file-based persistence (initial version)
- Data Format: JSON (RESTful design)
- Build Tool: Maven
- IDE: Visual Studio Code

---

## API Endpoints

You can find the detailed endpoint documentation in the `src/main/java/.../controller` package.

Typical endpoints include:

- `GET /pets` – Get all pets  
- `POST /pets` – Add a new pet  
- `PUT /pets/{id}` – Update pet info  
- `DELETE /pets/{id}` – Remove a pet  

Each pet includes:
- Name  
- Breed  
- Age (in months)  
- Weight (kg)  
- Gender  
- Last vaccinated (in months)  
- Microchipped status  
- Owner name  

---

## Testing & Integration

The API is designed to be consumed by the PetCareLib library, which wraps the endpoints and provides simple method calls for mobile developers.

---

## Future Extensions

- Full authentication layer (JWT or OAuth)
- Persistent database integration (e.g. PostgreSQL or MongoDB)
- Medical records and reminders
- Role-based access (vet, owner, admin)

---

## Contributing

If you'd like to suggest improvements or use this structure for your own pet-based apps, feel free to fork the repo and open a pull request.

---

## Related Projects

- PetCareLib – Android library wrapper for this API  
- PetCare App – Mobile frontend that integrates both SDK and API

---
