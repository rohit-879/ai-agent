# 🧠 COGNITIVE AI MANUFACTURING AGENT (IOT INDUSTRY AUTOMATION)

This project represents a **real-time intelligent automation system** designed for **Industrial IoT environments**. It provides a complete solution for monitoring, analyzing, alerting, self-healing, and visualizing machine and sensor data.

---

## 🔁 Simplified System Flow

```mermaid
flowchart LR
    A[📡 DataStreamX<br/>(Apache StreamPipes)] --> B[🧠 AI Agents<br/>(Node.js + Python)]
    B --> C[🔔 HookPilot<br/>(ActivePieces Webhooks)]
    B --> D[📊 React Dashboard<br/>(Monitoring UI)]

    subgraph A_desc [ ]
        direction TB
        A1[Collects data from IoT sensors via MQTT]
        A2[Triggers Kafka events for processing]
    end
    A --> A_desc

    subgraph B_desc [ ]
        direction TB
        B1[Processes streaming data]
        B2[Performs anomaly detection and auto-fix]
    end
    B --> B_desc

    subgraph C_desc [ ]
        direction TB
        C1[Sends real-time alerts]
        C2[Supports Telegram, Slack, Email, etc.]
    end
    C --> C_desc

    subgraph D_desc [ ]
        direction TB
        D1[Displays KPIs, Alerts, and Graphs]
        D2[Provides configuration and insights]
    end
    D --> D_desc
