
# 2. Part B — Configuring the LAN

## 2.1 Static IP Configuration
### Pi A (192.168.50.1)
> Insert screenshot here
<img width="1340" height="400" alt="image" src="https://github.com/user-attachments/assets/c5483972-1632-4257-a7be-4f3e8022762c" />

### Pi B (192.168.50.2)
> Insert screenshot here
<img width="1340" height="400" alt="image" src="https://github.com/user-attachments/assets/d5fc045c-17e4-45a0-a9d3-c5ffdd4b3068" />

## 2.2 Explanation
Explain:
- What is a static IP address?
- A static IP address is an IP address that is manually assigned to a computer or device. It does not change automatically.
- 
- Why both devices cannot use the same address
- Because each device on the same network must have its own unique IP address. If two devices use the same address, it causes an IP conflict.
- 
- Why we use /24
- We use /24 because it means the subnet mask is 255.255.255.0. It allows up to 254 devices to have unique IP addresses in the network.

