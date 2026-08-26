# Network & Web Reconnaissance Methodology

## Category: Web Directory Enumeration (DirBuster)
**Purpose:** Utilizes a graphical multi-threaded application to brute-force web application directories and filenames to expose unlinked administrative assets.

### Operational Process:
1. **Target Identification:** Configured the target host URL parameter pointing to the target web application asset (`http://fakebank.com`).
2. **Wordlist Selection:** Loaded a native directory wordlist into the utility to programmatically map valid path patterns.
3. **Directory Brute-Forcing:** Initiated the multi-threaded scanning engine to run automated HTTP requests against the backend web server.
4. **Attack Surface Discovery:** Analyzed the real-time response tree to discover an exposed, unauthorized bank transfer panel (`/bank-transfer-page`).





# Blue Team & Security Operations (SOC) Methodology

## Category: Threat Detection & Log Analysis
**Purpose:** Programmatically analyzing centralized system event logs within a Security Information and Event Management (SIEM) dashboard to detect, isolate, and remediate unauthorized infrastructure intrusion attempts.

### Operational Process:
1. **Log Ingestion Auditing:** Monitored real-time network and authentication logs collected from border firewalls and internal application servers.
2. **Anomaly Identification:** Detected a high-frequency spike in failed authentication requests originating from a single external IP address.
3. **Attack Classification:** Diagnosed the pattern as an active **Automated Credential Stuffing / Brute-Force Attack** attempting to breach user accounts.
4. **Incident Containment:** Executed remediation protocols by isolating the attacking IP address at the firewall layer, neutralizing the active thread, and maintaining enterprise infrastructure availability.