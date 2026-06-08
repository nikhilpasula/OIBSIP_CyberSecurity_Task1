# Task 1 - Basic Network Scanning with Nmap

## Objective

To perform a network scan on a local machine using Nmap and identify open ports and running services.

## Tool Used

* Nmap 7.99
* Windows Command Prompt

## Steps Performed

### 1. Installed Nmap

Verified the installation using:

```bash
nmap --version
```

### 2. Performed a Basic Network Scan

Executed:

```bash
nmap localhost
```

This scan identified open ports on the local machine.

### 3. Performed Service Detection

Executed:

```bash
nmap -sV localhost
```

This scan detected the services running on the identified ports.

### 4. Saved Scan Results

Executed:

```bash
nmap -sV localhost > nmap_scan_results.txt
```

The output was saved for analysis and documentation.

## Findings

| Port    | State | Service                       | Significance                                                                                                                    |
| ------- | ----- | ----------------------------- | ------------------------------------------------------------------------------------------------------------------------------- |
| 135/TCP | Open  | Microsoft Windows RPC (MSRPC) | Enables communication between Windows applications and services. Commonly used for system administration and remote management. |
| 445/TCP | Open  | Microsoft-DS (SMB)            | Used for file and printer sharing across Windows networks. Improperly secured SMB services may become security risks.           |

## Screenshots Included

1. Nmap Installation Verification
2. Basic Network Scan
3. Service Detection Scan

## Learning Outcome

Learned how to use Nmap to discover open ports, identify running services, and understand their significance from a cybersecurity perspective.

## Conclusion

The network scan successfully identified open ports and services running on the local machine. Nmap proved to be an effective tool for network reconnaissance and service enumeration. Understanding exposed services helps security professionals assess potential attack surfaces and improve system security.
