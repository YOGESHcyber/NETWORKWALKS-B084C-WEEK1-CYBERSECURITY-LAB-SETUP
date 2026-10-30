# NETWORKWALKS-B084C-WEEK1-CYBERSECURITY-LAB-SETUP
Cyber- lab-setup

**Project:** Cybersecurity Home Lab  
**Focus:** Virtualization, Kali Linux Installation, Network Configuration and Connectivity Testing  
**Platform:** Oracle VirtualBox  
**Operating System:** Kali Linux

## 1. Project Overview

Today, I built the room where the real work will happen.

As part of my cybersecurity learning journey, I dedicated Week 1 to building and configuring my own virtual cybersecurity laboratory.

Before moving into penetration testing, network analysis and defensive security, I wanted to establish a stable and isolated environment where I could safely learn, experiment and practice.

This week was about building the foundation.

## 2. Objectives

The main objectives were to:

- Set up a functional virtualization environment.
- Install and configure Kali Linux.
- Establish a private NAT Network.
- Create a clean virtual machine snapshot.
- Configure and verify network settings.
- Test internet connectivity and DNS resolution.

## 3. Tasks Completed

- [x] Installed and configured Oracle VirtualBox.
- [x] Imported and configured Kali Linux.
- [x] Created and configured a private NAT Network.
- [x] Created a clean virtual machine snapshot.
- [x] Configured and verified Kali Linux network settings.
- [x] Tested network connectivity.
- [x] Tested DNS resolution.

## 4. Tools and Technologies

| Tool | Purpose |
|---|---|
| Oracle VirtualBox | Virtualization |
| Kali Linux | Cybersecurity learning environment |
| NetworkManager | Network configuration |
| nmcli | Network management through CLI |
| Linux Terminal | Command-line administration |

## 5. Practical Commands Used

### Modify network connection settings
```bash
sudo nmcli connection modify "Wired connection 1" ipv4.dad-timeout 0
```

### Deactivate network connection
```bash
sudo nmcli connection down "Wired connection 1"
```

### Reactivate network connection
```bash
sudo nmcli connection up "Wired connection 1"
```

### Verify network devices
```bash
nmcli device status
```

### Check IP configuration
```bash
ip addr
```

### Test network connectivity
```bash
ping -c 4 8.8.8.8
```

### Test DNS resolution
```bash
ping -c 4 google.com
```

## 6. Key Learning Outcomes

This week's practical work helped me understand:

1. How virtualization provides an environment for cybersecurity practice.
2. How Kali Linux can be configured inside a virtual machine.
3. The importance of network isolation when building a lab.
4. How to manage network connections using NetworkManager.
5. How to inspect IP configuration.
6. The difference between testing IP connectivity and DNS resolution.
7. Why snapshots are useful for restoring a clean lab environment.

## 7. Challenges and Troubleshooting

One of the practical tasks involved configuring the Kali Linux network connection.

I used NetworkManager's command-line utility (`nmcli`) to modify the connection settings, deactivate the connection and reactivate it.

The commands returned successful activation messages.

This exercise reinforced the importance of troubleshooting systematically instead of randomly changing network settings.

## 8. Screenshots and Evidence

Screenshots documenting the following stages are included in the `screenshots/` directory:

<img width="1365" height="720" alt="Screenshot 2026-10-31 000836" src="https://github.com/user-attachments/assets/b0fd1eaf-9a6d-42d5-b0c1-49ea3f873313" />
<img width="1365" height="721" alt="Screenshot 2026-10-31 000615" src="https://github.com/user-attachments/assets/b94f0fe6-4d91-4286-9b7f-59a9b836b2b0" />
<img width="1366" height="643" alt="Screenshot_2026-10-30_13_00_25" src="https://github.com/user-attachments/assets/7ba38320-f603-41eb-b5df-e9382feecfe4" />
<img width="1366" height="643" alt="Screenshot_2026-10-30_13_16_30" src="https://github.com/user-attachments/assets/c0add055-0b94-4e20-9a96-b0d51ed15062" />
<img width="1366" height="643" alt="Screenshot_2026-10-30_14_43_32" src="https://github.com/user-attachments/assets/70fe5224-a4d2-4d9a-a493-c661d4b240bc" />

- VirtualBox configuration.
- Kali Linux environment.
- NAT Network configuration.
- Network connection management.
- Connectivity and DNS testing.

## 9. What's Next?

With the virtual lab established, my next objectives are:

- Strengthen my Linux command-line skills.
- Explore networking fundamentals.
- Practice IP addressing, ports and protocols.
- Introduce Wireshark for network traffic analysis.
- Begin basic defensive security and log analysis.

Week 1 was a reminder that every practical cybersecurity skill starts with a solid foundation.

**The environment is ready. Now the real learning begins.**

---

*This project is part of my ongoing beginner cybersecurity and SOC analyst learning journey.
