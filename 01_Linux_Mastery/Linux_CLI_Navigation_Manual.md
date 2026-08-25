# Network & Web Reconnaissance Methodology

## Category: Web Directory Enumeration (DirBuster)
**Purpose:** Utilizes a graphical multi-threaded application to brute-force web application directories and filenames to expose unlinked administrative assets.

### Operational Process:
1. **Target Identification:** Configured the target host URL parameter pointing to the target web application asset (`http://fakebank.com`).
2. **Wordlist Selection:** Loaded a native directory wordlist into the utility to programmatically map valid path patterns.
3. **Directory Brute-Forcing:** Initiated the multi-threaded scanning engine to run automated HTTP requests against the backend web server.
4. **Attack Surface Discovery:** Analyzed the real-time response tree to discover an exposed, unauthorized bank transfer panel (`/bank-transfer-page`).