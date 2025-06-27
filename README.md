# Cyber Security Internship - Task 4: Firewall Setup using UFW

## Objective

Set up and manage a basic firewall on Linux using UFW. The task involved blocking/allowing ports, testing traffic, and understanding how firewall rules help secure a system.

---

##  Tools Used

- Linux (Parrot OS)
- UFW (Uncomplicated Firewall)
- Netcat (for testing port connections)

---

## Steps I Followed

### 1. Enable UFW

sudo ufw enable

### 2. Check Current Rules

sudo ufw status verbose

### 3. Set Default Rules

sudo ufw default deny incoming
sudo ufw default allow outgoing

### 4. Allow Essential Services

sudo ufw allow ssh
sudo ufw allow http
sudo ufw allow https

### 5. Block Telnet (Port 23)

sudo ufw deny 23

### 6. Test with Netcat

nc -zv localhost 23

### 7. Limit SSH to Prevent Brute Force

sudo ufw limit ssh

### 8. Turn on Logging

sudo ufw logging on

### 9. Remove Test Rule

sudo ufw delete deny 23

(Screenshots Added )
