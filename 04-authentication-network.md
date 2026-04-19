# Authentication & Network Interaction (Level 16–20)

This section shifts focus from local file handling to network-based interactions and authentication methods.  
It introduces how services run on ports, how secure connections work, and how access can depend on more than just passwords.

---

## Level 16

**Goal:**  
Find the correct port that returns useful data.

**Concept:**  
Scanning for active services.

**Approach:**  
Used `nmap` to scan a range of ports and identify which ones are open and running services.

**Why it works:**  
`nmap` helps discover open ports and the services running on them, which is essential for interacting with unknown systems.

**Key Takeaway:**  
Before interacting with a system, you need to know what services are available.

---

## Level 17

**Goal:**  
Identify the correct response from multiple SSL-enabled ports.

**Concept:**  
Secure connections using SSL/TLS.

**Approach:**  
Used `openssl s_client` to connect to SSL-enabled ports and inspect responses.

**Why it works:**  
Some services require encrypted connections. `openssl` allows interaction with such services.

**Key Takeaway:**  
Not all services respond to plain connections—some require secure communication.

---

## Level 18

**Goal:**  
Access the next level despite restricted shell behavior.

**Concept:**  
Bypassing limited shell environments.

**Approach:**  
Used SSH with a command to directly execute and retrieve the required file instead of relying on an interactive shell.

**Why it works:**  
Even
