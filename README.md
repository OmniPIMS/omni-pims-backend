# OmniPIMS Backend  
Node.js + Express API

OmniPIMS Backend is the core service responsible for dynamic entity modeling, schema definition, attribute management, and runtime storage operations.

It provides a plug-and-play API for building product-driven or catalog-driven applications with dynamic data structures.

## 🚀 Features
- Dynamic schema definitions (no need to redeploy)
- Parameterized attributes with multiple data types
- Entity CRUD with flexible validation
- Schema versioning
- Extensible modular design
- REST API
- Docker-ready deployment

## 🛠 Tech Stack
- Node.js (LTS)
- Express.js
- TypeScript (optional in future roadmap)
- MongoDB or PostgreSQL (pluggable storage layer)
- Docker

## 📂 Project Structure
/src
/schemas -> schema definitions & validation
/entities -> entity CRUD logic
/routes -> express route handlers
/config -> environment, database, settings
index.js -> app bootstrap
/docs
/tests
Dockerfile
.env.example


## ▶ Running Locally

### Install
``npm install``


### Start
``npm run dev``


### Environment Variables
``Copy `.env.example` → `.env` and configure:``
``PORT=3000``
``DB_URI=mongodb://localhost:27017/opims``


## 🐳 Docker
Build:
``docker build -t opims-backend .``

Run:
``docker run -p 3000:3000 opims-backend``
## 📄 License
Apache 2.0 License  
Enterprise plugins/modules are proprietary and licensed separately.
