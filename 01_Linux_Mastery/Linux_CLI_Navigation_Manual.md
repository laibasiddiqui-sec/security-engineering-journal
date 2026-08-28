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





## Category: Encrypted Session Initialization & Local File System Auditing
**Target Environment:** OverTheWire Bandit - Level 0 to Level 1 Breach  
**Objective:** Establishing secure cryptographic network tunnels and executing low-level directory enumeration to extract targeted asset tokens.

### Operational Sequence & Command Architecture:
1. **Secure Shell Tunneling (`ssh`):** Initialized an encrypted terminal session using the Secure Shell protocol directed at a non-standard entry point (`Port 2220`). Authenticated via low-privilege system parameters to bypass perimeter barriers and establish an interactive remote bash environment.
2. **Environment Prompt Analysis:** Deconstructed the interactive prompt string (`bandit0@bandit:~$`) to verify user session context, target hostname boundaries, and active path orientation within the user home directory persistence layer.
3. **Directory Surface Enumeration (`ls`):** Executed directory enumeration commands to scan the active storage container file system, exposing an unlinked, non-executable data asset file containing baseline access criteria.
4. **Data Content Extraction (`cat`):** Deployed core text manipulation streams to read the raw data payload within the target asset file, successfully isolating the Level 1 cryptographic access validation token: `[REDACTED_ACCESS_HASH]`.
5. **Session Termination (`exit`):** Cleared active system input lines and initiated clean socket teardown procedures to safely close the encrypted remote network channel.