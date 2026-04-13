*This project has been created as part of the 42 curriculum by jgomez-d.*

# NetPractice

## Description

NetPractice is a practical networking exercise designed to introduce the fundamentals of computer networking. The goal is to configure 10 small-scale simulated networks by correctly assigning IP addresses, subnet masks, and default gateways so that all devices can communicate properly.

Through this project, you gain hands-on experience with TCP/IP addressing, understand how routers and switches interconnect devices, and learn how to troubleshoot network configurations using logs and diagnostic feedback provided by the training interface.

## Instructions

### Running the training interface

1. Download and extract the project files to any folder of your choice.
2. Open a terminal in that folder and run the launch script:

```bash
bash run.sh
```

This will start a local web server and open the NetPractice interface in your default browser.

If `run.sh` does not work, you can start the server manually:

```bash
python3 -m http.server 49242
```

Then navigate to `http://localhost:49242` in your browser.

### Using the interface

- Enter your login (`jgomez-d`) in the provided field to load your personal configuration.
- Alternatively, use the **evaluation** tab to generate a random configuration for practice.
- For each level, modify the unshaded fields to fix the network so it functions correctly.
- Use the **[Check again]** button to verify your configuration.
- Use the **[Get my config]** button to download and save your configuration for each level.

### Exporting and submitting

Once a level is completed, export the configuration file using **[Get my config]** before moving to the next level. This must be done for all 10 levels.

### Submission requirements

Place the 10 exported configuration files (one per level) at the root of your Git repository. Only the work present in your repository will be evaluated.

> **Note:** During the defense, you will be asked to complete 3 random levels within a limited time. No external tools are allowed, except for a simple calculator such as `bc`.

## Resources

### Networking concepts studied

- **TCP/IP addressing** — How IP addresses are structured and assigned to devices on a network.
- **Subnet masks** — How subnet masks determine which portion of an IP address identifies the network and which identifies the host.
- **Default gateways** — The role of a gateway in routing traffic between different networks.
- **Routers and switches** — How routers forward packets between networks and how switches connect devices within the same network.
- **OSI model layers** — The conceptual framework describing how data travels through a network, from physical transmission to application-level communication.
- **CIDR notation** — A compact way of expressing IP address ranges and subnet sizes.

### References

- [Cisco Networking Basics](https://www.netacad.com/courses/networking/networking-basics)
- [Subnetting Practice — Professor Messer](https://www.professormesser.com/network-plus/n10-008/n10-008-video/subnetting-part-1/)
- [IP Addressing and Subnetting for New Users — Cisco](https://www.cisco.com/c/en/us/support/docs/ip/routing-information-protocol-rip/13788-3.html)
- [Subnet Mask Cheat Sheet](https://www.aelius.com/njh/subnet_sheet.html)
- [OSI Model Explained — Cloudflare](https://www.cloudflare.com/learning/ddos/glossary/open-systems-interconnection-model-osi/)

### Use of AI

Claude (claude.ai) was used during this project in the following ways:

- **Understanding networking concepts:** Several core concepts such as subnetting, CIDR notation, and the role of the default gateway were not fully clear at the start of the project. Claude was used as a learning resource to get clear and concrete explanations of these topics, which were then validated through practice in the interface and discussion with peers.
- **README template generation:** Claude was used to generate an initial template for this README file following the structure required by the project guidelines. The content was then reviewed, adapted, and completed by me to accurately reflect the project and my own experience with it.

All AI-generated content was reviewed and understood before being used. Peer review was also sought to catch any inaccuracies or gaps.
