# Discovery Service (Eureka)

**Discovery Service** is the central registry in the **MicroServiceGrid** ecosystem.  
It allows microservices to automatically register and discover each other, enabling dynamic service lookup without hardcoded URLs.

---

## 🚀 Features

- Service registration with automatic deregistration on shutdown
- Dynamic service discovery for REST clients
- Load balancing between service instances
- Integration with API Gateway and all core services
- Key component for resilient inter-service communication

---

## 🛠️ Tech Stack

- **Java 21**
- **Spring Boot 3**
- **Spring Cloud Netflix Eureka**
- **Docker & Kubernetes**
- **GitHub Actions** for CI/CD

---

## 🧩 Service Integration

All microservices (Order, Inventory, Product, Gateway) register here.

Discovery Service provides:
- ✅ REST clients dynamically discover active service instances
- ✅ Heartbeat registration and health checks
- ✅ Load balancing between service instances
---
## ⚙️ Running Locally

1️⃣ Clone the repository:
```bash
git clone https://github.com/Andrij72/discovery-service.git
```
2️⃣ Start using Docker:
```bash
docker-compose -f docker-compose-examples/docker-compose.dockerfile.yml up -d
```
3️⃣ Open Eureka Dashboard:

http://localhost:8761

🌐 Dashboard
Eureka UI shows all registered services, their status, and instance metadata.

### 👨‍💻 Author
Andrij72 — microservice architecture, event-driven design, and cloud-native engineering.
