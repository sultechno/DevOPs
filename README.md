# 🛠️ MySQL High Availability & Monitoring

Welcome to the **MySQL High Availability, Replication & Monitoring** repository.  
This project contains documentation, configurations, and monitoring dashboards to help you build a resilient and scalable MySQL setup.

---

## 📚 Documentation (Wiki)

All guides are available in the **[Wiki Section](./wiki/)**:

- [Galera Cluster](./wiki/galera-cluster.md)  
- [MySQL Replication (GTID & XID)](./wiki/replication-gtid-xid.md)  
- [Binary Logs & PITR](./wiki/binlogs-pitr.md)  
- [Master → Slave Replication](./wiki/master-slave.md)  
- [Master ↔ Master Replication](./wiki/master-master.md)  
- [Database Name Rewrite](./wiki/replicate-rewrite-db.md)  

Each section includes step-by-step setup, configuration snippets, and best practices.

---

## 📊 Grafana Dashboards

The `grafana-dashboards/` folder contains JSON dashboard definitions ready to be imported into Grafana.

- **All Servers Dashboard**  
  A single dashboard showing metrics (CPU, memory, disk, MySQL status) from **all MySQL instances**.

- **Group Filter Dashboard**  
  Dashboard with filtering options to view metrics by **group name** (e.g., `db-cluster`, `replicas`, `analytics`).  
  This makes it easier to analyze performance across clusters or environments.

### Importing Dashboards
1. Open Grafana → *Dashboards* → *Import*.  
2. Upload JSON files from `grafana-dashboards/`.  
3. Adjust Prometheus data source if needed.  

---

## 🚀 Features
- End-to-end **MySQL HA setup** (Galera, Master-Slave, Master-Master).  
- **Replication tuning** with GTID and XID examples.  
- **Disaster Recovery** using Binlogs & PITR.  
- **Monitoring Dashboards** for instances and groups.  

---

## ✅ Best Practices
- Always secure replication users with strong passwords.  
- Test PITR restores regularly.  
- Use GTID replication where possible for easier failover.  
- Keep Grafana dashboards versioned in Git for consistency.  

---

## 🔗 Resources
- [MySQL Documentation](https://dev.mysql.com/doc/)  
- [MariaDB Galera Cluster Docs](https://mariadb.com/kb/en/what-is-mariadb-galera-cluster/)  
- [Grafana Docs](https://grafana.com/docs/)  

---

📌 **Maintainers**: Suleman  
📜 **License**: MSJ
