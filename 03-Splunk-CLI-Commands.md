# 🧩 Lab 3 — Exploring Splunk Through the CLI

After successfully installing and running **Splunk Enterprise** on the Linux server, I explored how to manage and interact with Splunk using its **Command-Line Interface (CLI)**. The CLI allows administrators to perform key operations such as starting, stopping, restarting, and monitoring the Splunk service — as well as executing searches directly from the terminal.

---

## ⚙️ Step 1: Navigating to Splunk’s CLI

All Splunk administrative commands are executed from within the Splunk installation directory:


I switched to this directory before running any CLI commands:

```bash
cd /opt/splunk/bin

```

## ⚙️ Step 2: Common Splunk CLI Commands

1. Start Splunk

The splunk start command initializes the Splunk service and makes it accessible via the web interface (http://coffely:8000).


```bash

./splunk start

```
This command launches the necessary processes and opens key ports:

HTTP: 8000

Management: 8089

App Server: 8065

KV Store: 8191

Once startup checks are complete, Splunk displays:

```bash

The Splunk web interface is at http://coffely:8000

```


2. Stop Splunk

The splunk stop command stops all running Splunk services safely.

```bash

./splunk stop

```
This ensures all background Splunk processes are properly terminated.

![Image Alt](https://github.com/Balasankkar/Splunk-Full-SIEM-SOC-Lab/blob/374a8d80d3f4b7658b95daf6e1f7b8f4f39f8204/Screenshots/Figure1%2CL3.png)
Figure 1 — Starting and Stopping the Splunk service via CLI.

3. Restart Splunk

Used when changes are made to configuration files or apps.
It first stops all running processes and then starts them again.

```bash
./splunk restart
```
![Image Alt](https://github.com/Balasankkar/Splunk-Full-SIEM-SOC-Lab/blob/374a8d80d3f4b7658b95daf6e1f7b8f4f39f8204/Screenshots/Figure2%2CL3.png)
Figure 2 — Using restart command.


4. Check Splunk Status
The splunk status command verifies whether Splunk is running and displays process IDs (PIDs) for active Splunk services.

```bash

./splunk status

```
Example output: 

```bash

splunkd is running (PID: 2158)
splunk helpers are running (PIDs: 2159 2301 2351 2437)

```
![Image Alt](https://github.com/Balasankkar/Splunk-Full-SIEM-SOC-Lab/blob/374a8d80d3f4b7658b95daf6e1f7b8f4f39f8204/Screenshots/Figure3%2CL3.png)
Figure 3 — Using status command

5. Add One-Shot Event

The splunk add oneshot command is used to manually add a single event to the Splunk index — helpful for testing log ingestion.

```bash

./splunk add oneshot

```

6. Search Data via CLI

Splunk’s search command allows quick searches directly from the terminal using Splunk’s Search Processing Language (SPL).

```bash

./splunk search coffely

```

7. Help Command

The splunk help command displays all available CLI options and syntax information.

```bash

./splunk help

```

This is the most important command for troubleshooting or exploring available functionality.

![Image Alt](https://github.com/Balasankkar/Splunk-Full-SIEM-SOC-Lab/blob/374a8d80d3f4b7658b95daf6e1f7b8f4f39f8204/Screenshots/Figure4%2CL3.png)
Figure 4 — viewing help options from the CLI.

## ✅ Outcome

Learned key Splunk CLI commands for managing services and performing searches.

Verified that Splunk can be controlled entirely through the terminal.

Successfully ran test searches and confirmed system operation via CLI.

