<div align="center">

# 🚀 AI-PORT-X

### Autonomous Multi-Agent Intelligence System for End-to-End Smart Port Operations Orchestration

**"Where Six AI Agents Run Your Port, Autonomously."**

[![Python](https://img.shields.io/badge/Python-3.10+-3776AB?style=for-the-badge&logo=python&logoColor=white)](https://python.org)
[![FastAPI](https://img.shields.io/badge/FastAPI-0.109-009688?style=for-the-badge&logo=fastapi&logoColor=white)](https://fastapi.tiangolo.com)
[![React](https://img.shields.io/badge/React-18-61DAFB?style=for-the-badge&logo=react&logoColor=black)](https://reactjs.org)
[![Gemini](https://img.shields.io/badge/Gemini-API-4285F4?style=for-the-badge&logo=google&logoColor=white)](https://ai.google.dev)
[![SQLite](https://img.shields.io/badge/SQLite-3-003B57?style=for-the-badge&logo=sqlite&logoColor=white)](https://sqlite.org)
[![License](https://img.shields.io/badge/License-MIT-yellow?style=for-the-badge)](LICENSE)

</div>

---

## 📖 Overview

**AI-PORT-X** is a next-generation, AI-powered smart port management platform that leverages the power of **Collaborative Multi-Agent Systems (MAS)** and **Large Language Models (LLMs)** to autonomously orchestrate every critical operation within a modern maritime port ecosystem.

Traditional port operations rely heavily on manual coordination between multiple stakeholders — ship operators, crane operators, customs officials, warehouse managers, and truck dispatchers — leading to delays, inefficiencies, bottlenecks, and increased operational costs.

**AI-PORT-X eliminates this fragmentation** by deploying **six intelligent autonomous agents** that communicate, reason, negotiate, and optimize decisions in real-time — powered by **Google Gemini LLM**.

---

## 🎯 Problem Statement

Modern ports handle thousands of containers daily, yet suffer from:

- ❌ Delayed vessel turnaround times
- ❌ Idle crane hours & poor resource allocation
- ❌ Slow customs clearance processes
- ❌ Warehouse over-occupancy & inventory mismatches
- ❌ Truck queue congestion at port gates
- ❌ Lack of real-time visibility across operations
- ❌ No intelligent coordination between departments

---

## 💡 Our Solution

AI-PORT-X introduces a **collaborative multi-agent AI framework** where each agent specializes in one domain but works together as a unified brain.

| # | Agent | Responsibility | Intelligence |
|---|-------|---------------|-------------|
| 🚢 | **Ship Agent** | Arrival, docking & departure scheduling | Predictive ETA, berth allocation |
| 🏗️ | **Crane Agent** | Crane allocation & container handling | Load balancing, priority scheduling |
| 🛃 | **Customs Agent** | Cargo clearance & documentation | Risk assessment, compliance check |
| 🏭 | **Warehouse Agent** | Space allocation & inventory tracking | Occupancy optimization, slotting |
| 🚛 | **Truck Agent** | Dispatch & route coordination | Queue management, route optimization |
| 📦 | **Cargo Agent** | End-to-end cargo lifecycle coordination | Cross-agent negotiation |

All agents are powered by **Google Gemini LLM** and communicate through a central **Orchestrator** that ensures smooth, conflict-free, and optimized decision-making.

---

## 🏗️ System Architecture

```
┌─────────────────────────────────────────────────────────┐
│                    REACT FRONTEND                       │
│  Dashboard │ Ships │ Cranes │ Customs │ Simulation      │
└────────────────────────┬────────────────────────────────┘
                         │ REST API + WebSocket
┌────────────────────────▼────────────────────────────────┐
│              FASTAPI BACKEND (Python)                   │
│  ┌──────────────────────────────────────────────────┐   │
│  │           AGENT ORCHESTRATOR (Core)              │   │
│  │  ┌──────┐ ┌──────┐ ┌──────┐ ┌──────┐ ┌──────┐   │   │
│  │  │ Ship │ │Crane │ │Custom│ │Wareh.│ │Truck │   │   │
│  │  └──┬───┘ └──┬───┘ └──┬───┘ └──┬───┘ └──┬───┘   │   │
│  │     └────────┴────────┴────────┴────────┘       │   │
│  │                    │                             │   │
│  │             ┌──────▼──────┐                      │   │
│  │             │ Gemini LLM  │                      │   │
│  │             └─────────────┘                      │   │
│  └──────────────────────────────────────────────────┘   │
└────────────────────────┬────────────────────────────────┘
                         │ SQLAlchemy ORM
┌────────────────────────▼────────────────────────────────┐
│                  SQLite DATABASE                        │
│  Ships │ Cranes │ Customs │ Warehouses │ Trucks        │
│  Cargo │ Containers │ AgentLogs │ Simulations          │
└─────────────────────────────────────────────────────────┘
```

---

## 🛠️ Technology Stack

### Frontend
| Technology | Purpose |
|-----------|---------|
| **React 18** | UI Library |
| **Vite** | Build Tool |
| **Tailwind CSS** | Styling |
| **Recharts** | Data Visualization |
| **Framer Motion** | Animations |
| **React Router** | Routing |
| **Axios** | HTTP Client |
| **React Hot Toast** | Notifications |

### Backend
| Technology | Purpose |
|-----------|---------|
| **Python 3.10+** | Programming Language |
| **FastAPI** | Web Framework |
| **Uvicorn** | ASGI Server |
| **SQLAlchemy** | ORM |
| **Pydantic** | Data Validation |
| **WebSockets** | Real-time Updates |
| **JWT** | Authentication |

### AI / Database
| Technology | Purpose |
|-----------|---------|
| **Google Gemini API** | LLM for Agent Reasoning |
| **gemini-1.5-flash** | Fast, CPU-friendly model |
| **SQLite** | Lightweight Database |

---

## ✨ Key Features

- ✅ **Six Autonomous Collaborative AI Agents**
- ✅ **Real-time Port Control Dashboard**
- ✅ **Live Ship Tracking & Berth Visualization**
- ✅ **Dynamic Crane Allocation Engine**
- ✅ **Customs Clearance Automation**
- ✅ **Warehouse Occupancy Optimizer**
- ✅ **Truck Queue & Dispatch Manager**
- ✅ **End-to-End Cargo Lifecycle Tracking**
- ✅ **Full Port Simulation Engine** (Ship → Delivery)
- ✅ **Agent Activity Feed with Reasoning Logs**
- ✅ **Interactive Analytics with Charts**
- ✅ **Modern Dark-Themed Glassmorphism UI**
- ✅ **JWT-Based Authentication**
- ✅ **WebSocket Live Streaming**
- ✅ **CPU-Friendly** (Gemini runs on cloud)

---

## 📁 Project Structure

```
ai-smart-port-management/
│
├── README.md
├── .gitignore
├── .env.example
├── docker-compose.yml
│
├── backend/
│   ├── main.py
│   ├── config.py
│   ├── database.py
│   ├── requirements.txt
│   ├── agents/
│   ├── models/
│   ├── schemas/
│   ├── routes/
│   ├── services/
│   ├── utils/
│   ├── core/
│   └── tests/
│
├── frontend/
│   ├── package.json
│   ├── vite.config.js
│   ├── tailwind.config.js
│   └── src/
│       ├── api/
│       ├── components/
│       ├── pages/
│       ├── context/
│       ├── hooks/
│       ├── routes/
│       └── utils/
│
├── database/
│   ├── schema.sql
│   ├── seed.sql
│   └── smart_port.db
│
└── docs/
    ├── ARCHITECTURE.md
    ├── API_DOCS.md
    └── SETUP_GUIDE.md
```

---

## 🚀 Getting Started

### Prerequisites

Make sure you have these installed:

- ✅ Python 3.10 or higher
- ✅ Node.js 18 or higher
- ✅ Git
- ✅ Google Gemini API Key ([Get it here](https://aistudio.google.com/app/apikey))

---

### 🔧 Backend Setup

```bash
# 1. Navigate to backend folder
cd backend

# 2. Create virtual environment
python -m venv venv

# 3. Activate virtual environment
# Windows:
venv\Scripts\activate
# Mac/Linux:
source venv/bin/activate

# 4. Install dependencies
pip install -r requirements.txt

# 5. Create .env file
# Copy .env.example to .env and add your Gemini API key

# 6. Run the server
uvicorn main:app --reload --port 8000
```

Backend will run at: **http://localhost:8000**
API Docs: **http://localhost:8000/docs**

---

### 🎨 Frontend Setup

```bash
# 1. Navigate to frontend folder
cd frontend

# 2. Install dependencies
npm install

# 3. Create .env file with backend URL

# 4. Run development server
npm run dev
```

Frontend will run at: **http://localhost:5173**

---

### 🔑 Environment Variables

Create `.env` file in `backend/` folder:

```env
GEMINI_API_KEY=your_gemini_api_key_here
DATABASE_URL=sqlite:///./smart_port.db
JWT_SECRET_KEY=your_super_secret_key
JWT_ALGORITHM=HS256
ACCESS_TOKEN_EXPIRE_MINUTES=60
```

---

## 📊 API Endpoints

| Method | Endpoint | Description |
|--------|----------|-------------|
| `GET` | `/api/dashboard/stats` | Get dashboard statistics |
| `GET` | `/api/ships` | List all ships |
| `POST` | `/api/ships` | Add new ship |
| `GET` | `/api/cranes` | List all cranes |
| `GET` | `/api/customs` | List customs clearances |
| `GET` | `/api/warehouses` | List warehouses |
| `GET` | `/api/trucks` | List trucks |
| `GET` | `/api/cargo` | List cargo shipments |
| `POST` | `/api/agents/orchestrate` | Trigger multi-agent workflow |
| `POST` | `/api/simulation/start` | Start port simulation |
| `WS` | `/ws/live` | WebSocket for live updates |

> 📘 Full API documentation available at `/docs` (Swagger UI)

---

## 🎬 How It Works

### Step 1: Ship Arrival
The **Ship Agent** detects incoming vessel, predicts ETA, and reserves a berth.

### Step 2: Crane Allocation
The **Crane Agent** analyzes cargo load, selects optimal crane, and schedules unloading.

### Step 3: Customs Clearance
The **Customs Agent** verifies documentation, performs risk assessment, and clears cargo.

### Step 4: Warehouse Assignment
The **Warehouse Agent** finds optimal storage slot based on cargo type and space.

### Step 5: Truck Dispatch
The **Truck Agent** assigns trucks, optimizes routes, and manages queue at gate.

### Step 6: Cargo Coordination
The **Cargo Agent** oversees the entire lifecycle and ensures smooth handoff between agents.

---

## 🌟 Impact & Benefits

| Metric | Improvement |
|--------|-------------|
| ⚡ Vessel Turnaround Time | **~40% faster** |
| ⚡ Idle Crane Hours | **~35% reduction** |
| ⚡ Customs Clearance | **~50% faster** |
| ⚡ Warehouse Utilization | **~30% improvement** |
| ⚡ Real-Time Visibility | **100% coverage** |

> *Note: These are simulated results from the built-in simulation engine.*

---

## 🎯 Industry Relevance

- **Domain**: Logistics & Maritime Supply Chain
- **Industry 4.0 Alignment**: Autonomous systems, AI-driven optimization
- **Real-World Applicability**: JNPT, Mundra, Singapore, Rotterdam ports
- **Future Scope**: Blockchain, Digital Twin, IoT sensors

---

## 🔮 Future Enhancements

- [ ] Blockchain-based cargo tracking
- [ ] Digital Twin for port visualization
- [ ] IoT sensor integration for real-time telemetry
- [ ] Voice-based agent commands
- [ ] Mobile app (React Native)
- [ ] Multi-port federation
- [ ] Advanced ML-based ETA prediction
- [ ] Drone-based cargo inspection

---

## 🧪 Testing

```bash
# Backend tests
cd backend
pytest

# Frontend tests
cd frontend
npm run test
```

---

## 🤝 Contributing

This project is currently for **educational and practice purposes**. Contributions, suggestions, and feedback are welcome!

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/AmazingFeature`)
3. Commit your changes (`git commit -m 'Add some AmazingFeature'`)
4. Push to the branch (`git push origin feature/AmazingFeature`)
5. Open a Pull Request

---

## 📜 License

This project is licensed under the **MIT License** — see the [LICENSE](LICENSE) file for details.

---

## 👨‍💻 Author

**Vishakha Patil**

- GitHub: [@vishakha2121](https://github.com/vishakha2121)
- Project Repo: [AI-PORT-X](https://github.com/vishakha2121/AI-PORT-X-Autonomous-Multi-Agent-Intelligence-System-for-End-to-End-Smart-Port-Operations)

---

## 🙏 Acknowledgements

- **Google Gemini API** for powering autonomous agent reasoning
- **FastAPI** for the blazing-fast backend framework
- **React & Vite** for the modern frontend experience
- **Tailwind CSS** for the stunning UI
- The open-source community for inspiration and tools

---

<div align="center">

### ⭐ If you like this project, please give it a star! ⭐

**Built with ❤️ for Smart Ports of Tomorrow**

```
╔══════════════════════════════════════════════════════════╗
║                                                          ║
║              🚀  A I - P O R T - X  🚀                  ║
║                                                          ║
║   "Six Minds. One Port. Zero Chaos."                    ║
║                                                          ║
╚══════════════════════════════════════════════════════════╝
```

</div>