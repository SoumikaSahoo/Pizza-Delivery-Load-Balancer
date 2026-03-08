🍕# Pizza-Delivery-Load-Balancer
A simulation of a load balancing system using pizza delivery drivers as backend servers.
The system distributes incoming delivery requests to the least busy driver, demonstrating how load balancing algorithms work in distributed systems.

This project helps visualize traffic distribution and resource management, concepts commonly used in modern infrastructure and cloud systems.

🚀 Features

🍕 Simulates incoming pizza delivery orders

⚖️ Automatically assigns deliveries to the least loaded driver

👨‍🍳 Add new drivers dynamically

🔄 Activate or deactivate drivers

📊 Real-time delivery tracking

🌐 Web dashboard built with Flask

🧠 Load Balancing Logic

The system uses a Least Load Scheduling Algorithm.

Each incoming order is assigned to the driver with the fewest active deliveries.

Example:

Driver A → 5 deliveries  
Driver B → 2 deliveries  
Driver C → 4 deliveries

Next order will be assigned to:

Driver B

This is similar to load balancing strategies used in production systems like NGINX, HAProxy, and Kubernetes services.

🏗 Project Structure
pizza-delivery-load-balancer
│
├── app.py
├── requirements.txt
├── Procfile
├── render.yaml
│
├── templates
│   ├── index.html
│   └── add_driver.html
│
└── static
    ├── style.css
    └── background.jpg
⚙️ Installation

Clone the repository:

git clone https://github.com/your-username/pizza-delivery-load-balancer.git
cd pizza-delivery-load-balancer

Install dependencies:

pip install -r requirements.txt

Run the application:

python app.py

Open your browser:

http://127.0.0.1:5000
🖥 Dashboard

The web dashboard allows you to:

Monitor active drivers

Track delivery assignments

Add or disable drivers

Observe how orders are distributed

📚 Concepts Demonstrated

This project demonstrates several core distributed systems and SRE concepts:

Load Balancing

Traffic Scheduling

Resource Allocation

Background Workers

Web Application Deployment

🛠 Technologies Used

Python

Flask

HTML/CSS

JavaScript

Threading (for delivery simulation)

🌟 Future Improvements

Possible enhancements:

Implement Round Robin Load Balancing

Implement Weighted Load Balancing

Add real-time charts

Add Docker containerization

Deploy with Kubernetes

Add Prometheus monitoring
