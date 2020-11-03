# The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services Dataset

This page is dedicated to the distribution of the dataset collected and used in the "The Dark (and Bright) Side of IoT" paper; by Ahmed Mohamed Hussain [^1], Gabriele Oligeri [^2], and Thiemo Voigt [^1].

[^1]: Department of Information Technology, Uppsala University, Uppsala, Sweden.
[^2]: Hamad Bin Khalifa University (HBKU) - College of Science and Engineering (CSE) - Division of Information and Computing Technology (ICT).

## The data collection has been performed accordingly to the following procedure:
- We adopted airodump-ng to identify the victim access point and the devices connected to it. 
- Identifying information such as MAC addresses and WiFi channel used by the devices in the network.
- Setting the Alfa card channel to the one used by the smart device.
- Using either [TCPDump] or [Wireshark] for traffic collection and filtering out the traffic generated from the access point to each of the IoT device. Using the MAC address obtained from the first step.
- Extract the time and packet size associated with each over-the-air message.

# Dataset 
Each dataset corrosponde to the following devices -- service:
- Amazon Echo -- Music
- Amazon Echo -- News
- Amazon Echo Dot -- Music
- Amazon Echo Dot -- News
- Google Nest Mini -- Music

### Each file contains the following columns:

- Raw Time: in seconds since beginning of capture
- Raw Packet size: in bytes

# License
GPL--3.0

[TCPDump]: <https://www.tcpdump.org>
[Wireshark]: <https://www.wireshark.org/>
