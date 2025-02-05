# 🚀 **Event Comms** - **Lightning Web Components (LWC)**

This project is a **Lightning Web Components (LWC)** application that demonstrates event communication in Salesforce. It consists of multiple components that interact using **custom events** to dynamically update and manage a counter.

## 📌 **Overview**

The application consists of the following components:

- **Numerator**: Displays the current and previous count.
- **RemoteControl**: Provides buttons to modify the counter (add, subtract, multiply).
- **Augmentor**: Allows setting a starting value for the counter.
- **Controls**: Centralized panel with action buttons.
- **Counts**: Displays the count state dynamically.

These components communicate using **Lightning events**, showcasing how child components update parent components.

## 🛠️ **Installation & Setup**

### **1️⃣ Prerequisites**

- A **Salesforce Developer Org** or a **Scratch Org**.
- **Salesforce CLI** installed.
- A connected **SFDX project**.

### **2️⃣ Clone the Repository**

```sh
git clone [https://github.com/theotheodoridis98/Event-Comms-LWC.git](https://github.com/theotheodoridis98/Event-Comms-LWC.git)
cd Event-Comms-LWC
3️⃣ Deploy to Salesforce
Bash

sf org login web -d -a my-devhub
sf org create scratch -f config/project-scratch-def.json -a my-scratch-org -d 30
sf project deploy start
sf org assign permset --name EventCommsPermissionSet
sf org open
For more details, see the Salesforce DX Developer Guide.

📂 Component Details

1️⃣ Numerator
Displays the current and previous count.
Listens for count updates from other components.
2️⃣ RemoteControl
Provides buttons to modify the counter:
➕ Add
➖ Subtract
✖ Multiply (2-6)
Dispatches custom events to update the numerator.
3️⃣ Augmentor
Allows setting a starting counter value via an input field.
4️⃣ Controls
Provides action buttons (➕ ➖ ✖) to modify the count.
Sends events to update the Numerator.
5️⃣ Counts
Displays the count state dynamically.
Listens for events to update automatically.

🚀 Features & Functionality

🔄 Real-time event-driven updates.

⚡ Efficient Lightning Data Binding.

🎨 Custom UI styling.

📡 Decoupled architecture using @api, @track, and event dispatching.


![image](https://github.com/user-attachments/assets/03a3bdfd-759e-43a0-9c12-43cf2afa59f0)

