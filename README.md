# The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services Dataset

This repository is dedicated to the distribution of the dataset collected and used in the "The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services" paper, accepted at [SPIoT 2020] in conjunction with [SpaCCS 2020]; by Ahmed Mohamed Hussain ([Uppsala University]), Gabriele Oligeri ([Hamad Bin Khalifa University]), and Thiemo Voigt ([Uppsala University]).

# Dataset 
### The data collection has been performed accordingly to the following procedure:
- We adopted [Airodump-ng] to identify the victim access point and the devices connected to it. 
- Identifying information such as MAC addresses and WiFi channel used by the devices in the network.
- Setting the Alfa card channel to the one used by the smart device.
- Using either [TCPDump] or [Wireshark] for traffic collection and filtering out the traffic generated from the access point to each of the IoT device. Using the MAC address obtained from the first step.
- Extract the time and packet size associated with each over-the-air message.

### Each dataset corrosponde to the following device -- service:
- Amazon Echo -- Music
- Amazon Echo -- News
- Amazon Echo Dot -- Music
- Amazon Echo Dot -- News
- Google Nest Mini -- Music

### Each file contains the following columns:

- Raw Time: in seconds since beginning of capture
- Raw Packet size: in bytes

## License
[GPL-3.0](https://github.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/blob/main/LICENSE)
[Uppsala University]: <https://www.it.uu.se/>
[Hamad Bin Khalifa University]: <https://www.hbku.edu.qa/en/division/information-computing-technology>
[TCPDump]: <https://www.tcpdump.org>
[Wireshark]: <https://www.wireshark.org/>
[Airodump-ng]: <https://www.aircrack-ng.org/doku.php?id=airodump-ng>
[SPIoT 2020]: <http://www.spaccs.org/spiot2020/>
[SpaCCS 2020]: <http://www.spaccs2020.com/>
