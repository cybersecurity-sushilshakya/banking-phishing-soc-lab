# Lab Architecture

## Network Configuration

### Ubuntu Desktop (Victim + SOC)

  <ul>Interface 1 (enp0s3): Bridged Adapter (Used for external connectivity)</ul>
  <ul>Interface 2 (enp0s8): NAT Network</ul>
  <ul>IP Address: 10.10.10.20/24</ul>

### Parrot OS (Attacker)
  <ul>Interface: NAT Network</ul>
  <ul>IP Address: 10.10.10.50/24</ul>

## Network Diagram

  Ubuntu Desktop (10.10.10.20)
   ├── Thunderbird Email Client
   ├── Snort IDS
   └── Wireshark Packet Analysis

         |
         | NAT Network
         v
  Parrot OS (10.10.10.50)
   ├──   FakeSMTP
   ├── SET Toolkit
   └── Apache Phishing Site


