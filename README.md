# ModbusTCP_sensor

**A lightweight Python service that reads Modbus TCP data and stores it in a database.**

---

## 🚀 Overview

This project simulates a Siemens PLC environment and demonstrates how to:

1. **Run a dummy Modbus TCP server** that generates synthetic sensor data.
2. **Build a Flask-based service** (`pyModbusTCP`) to periodically poll data.
3. **Store the readings** into a database (SQLite/PostgreSQL).
4. **Deploy everything via Docker & Docker‑Compose** for easy setup.

Ideal for learning how to integrate industrial systems (IIoT, SCADA) with modern backend tooling.

---

## 📦 Features

- **Modbus TCP Server**: Simulates register values that update every 500 ms  
- **Flask API**:  
  - `/` — health check  
  - `/read` — manual trigger to read Modbus registers  
- **Database Storage**: (PostgreSQL via Docker)  
- **Containerized Deployment**:  
  ```shell
  docker-compose up --build
