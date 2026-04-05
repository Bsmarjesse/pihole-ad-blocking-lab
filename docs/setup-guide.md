# Pi-hole Setup Guide

## Overview
This guide documents the deployment of Pi-hole as a network-wide DNS ad-blocking solution in a home lab environment.

---

## Environment
- Raspberry Pi
- Pi-hole installed via official script
- Router configured for DNS redirection
- IPv6 disabled to prevent DNS bypass

---

## Installation Steps

### 1. Install Pi-hole
```bash
curl -sSL https://install.pi-hole.net | bash


### 2. Assign Static IP
Configured a static IP address for the Raspberry Pi to ensure consistent DNS resolution.

Example:
10.0.0.5

---

### 3. Configure Router DNS
- Set router LAN DNS to Pi-hole IP address
- Removed secondary DNS entries to prevent bypass

---

### 4. Disable IPv6
Disabled IPv6 on the router to prevent DNS queries from bypassing Pi-hole filtering.

---

### 5. Verify Functionality
- Accessed Pi-hole web interface
- Confirmed DNS queries were being logged
- Verified ad blocking across multiple devices
