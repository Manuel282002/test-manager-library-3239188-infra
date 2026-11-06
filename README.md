# Manager Library — Infrastructure & Containers

This repository manages the isolated execution and deployment environment for the library ecosystem.

## Docker Compose Orchestration
A `docker-compose.yml` file has been implemented to automate environment provisioning:
- **Database Engine:** Official **PostgreSQL 16** container (lightweight Alpine version).
- **Network Isolation:** Dedicated bridge network configuration (`library_net`).
- **Data Persistence:** A named volume (`library_pg_data`) to guarantee immutability and indefinite retention of the historical transaction logs for loans and catalogs.
