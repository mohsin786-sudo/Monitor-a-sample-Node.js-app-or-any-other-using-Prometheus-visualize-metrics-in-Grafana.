# 📊 Monitor a Sample Node.js App using Prometheus and Grafana

This project demonstrates how to monitor a sample Node.js application using **Prometheus** for metrics collection and **Grafana** for visualization.

---

## 🛠️ Features

- 📈 Real-time metrics collection using Prometheus  
- 📊 Beautiful dashboards in Grafana  
- 🔧 Export metrics from a Node.js app using `prom-client`  
- 🐳 Dockerized setup using `docker-compose`  
- ✅ Easy to extend to other apps and services  

---

## 📁 Project Structure

. ├── app/                            # Sample Node.js app with Prometheus metrics │   ├── server.js                   # Main application code │   └── package.json ├── prometheus/                     # Prometheus configuration │   └── prometheus.yml ├── grafana/                        # Grafana provisioning │   └── dashboards/                 # JSON dashboards (optional) ├── docker-compose.yml             # Docker Compose setup └── README.md

---

## 🚀 Getting Started

### Prerequisites

- [Docker](https://docs.docker.com/get-docker/)
- [Docker Compose](https://docs.docker.com/compose/install/)

### 1. Clone the Repository

```bash
git clone https://github.com/mohsin786-sudo/Monitor-a-sample-Node.js-app-or-any-other-using-Prometheus-visualize-metrics-in-Grafana.git
cd Monitor-a-sample-Node.js-app-or-any-other-using-Prometheus-visualize-metrics-in-Grafana

2. Start the Stack

docker-compose up --build

> Prometheus: http://localhost:9090

Grafana: http://localhost:3000




Grafana login:

Username: admin

Password: admin (change after first login)



---

📌 Node.js App Metrics Endpoint

The Node.js app exposes metrics at:

http://localhost:8080/metrics

Sample metrics include:

HTTP request count

Request duration histogram

Custom counters and gauges



---

📊 Setting Up Grafana Dashboard

1. Open Grafana at http://localhost:3000


2. Add Prometheus as a data source (http://prometheus:9090)


3. Create a new dashboard or import one


4. Use metrics like http_requests_total, http_request_duration_seconds_bucket, etc.




---

🧼 Clean Up

To stop and remove all containers:

docker-compose down


---

📄 License

This project is licensed under the MIT License.

---

