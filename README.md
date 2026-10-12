# Pi-hole DNS Security Lab

## Overview

Configured Pi-hole as a DNS filtering server and troubleshot a Windows DNS bypass caused by IPv6.

## Lab Setup

- Windows 11
- Ubuntu Server
- Pi-hole
- Xfinity Gateway
- PowerShell
- Command Prompt

### Network
- PC: `10.0.0.29`
- Pi-hole: `10.0.0.53`
- Gateway: `10.0.0.1`
- Subnet: `255.255.255.0`

## Problem

Pi-hole worked when queried directly:

```cmd
nslookup doubleclick.net 10.0.0.53
