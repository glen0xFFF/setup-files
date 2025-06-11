# 🌐 MongoDB Replica Set Across Multiple Hosts

This guide walks you through setting up a MongoDB replica set with three nodes on separate servers or virtual machines.

## 🧾 Assumptions

| Node | Hostname              | IP             | Port  |
|------|-----------------------|----------------|-------|
| Node 1 (Primary)   | mongo1.example.com     | 192.168.1.101  | 27017 |
| Node 2 (Secondary) | mongo2.example.com     | 192.168.1.102  | 27017 |
| Node 3 (Secondary) | mongo3.example.com     | 192.168.1.103  | 27017 |

MongoDB is installed on all nodes.

---

## 🔧 Step 1: Configure Networking

Ensure all nodes can reach each other:

```bash
ping mongo2.example.com
ping mongo3.example.com
