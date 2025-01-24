# EGR226-Lab1

Ports and Threading

This lab demonstrates how to implement a simple port scanner in Python that uses multi-threading to scan a range (or list) of ports on a given host. By leveraging threads and a shared queue, the scanner can quickly identify which ports are open or closed. Key Features Socket Connections Uses Python’s socket module to attempt TCP connections on each specified port. Multi-Threading Spawns multiple threads (via threading.Thread) that each pull ports from a shared Queue, improving overall scan speed. Port Ranges & Modes Mode 1: Scans ports 1–1023 (commonly “well-known” ports). Mode 2: Scans ports 1–49152. Mode 3: Scans a predefined list of common service ports (e.g., 22, 25, 80, etc.). Mode 4: Scans user-entered ports via console input. Mode 5: Scans a custom set of ports from the lab instructions (FTP, SSH, SMTP, HTTP, etc.). Results Prints “Port X is open!” or “Port X is closed!” for each tested port, and then displays a final list of open ports.
