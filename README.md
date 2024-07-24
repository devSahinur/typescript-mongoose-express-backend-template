# Locating MongoDB Database on DigitalOcean Droplet

**Description**: Steps to find and access the MongoDB database on a DigitalOcean droplet.

---

## Instructions

1. **Access the Droplet:**
   - Log into the droplet using SSH:
     ```bash
     ssh [username]@[droplet_ip_address]
     ```

2. **Check MongoDB Status:**
   - Ensure MongoDB is running:
     ```bash
     sudo systemctl status mongod
     ```
   - If not running, start MongoDB:
     ```bash
     sudo systemctl start mongod
     ```

3. **Access MongoDB Shell:**
   - Enter the MongoDB shell:
     ```bash
     mongo
     ```

4. **List Databases:**
   - Display available databases:
     ```bash
     show dbs
     ```

5. **Access a Specific Database:**
   - Switch to a database:
     ```bash
     use [database_name]
     ```

6. **Check Collections:**
   - List collections in the database:
     ```bash
     show collections
     ```

**Note**: If there are issues accessing the database, check the MongoDB configuration file (`/etc/mongod.conf`) for the data directory or other configurations.
