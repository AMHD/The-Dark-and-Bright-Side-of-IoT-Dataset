# The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services -- Dataset

This repository is dedicated to the distribution of the dataset collected and used in ***The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services*** [paper], accepted at [SPIoT 2020] in conjunction with [SpaCCS 2020]; by Ahmed Mohamed Hussain ([Uppsala University]), Gabriele Oligeri ([Hamad Bin Khalifa University]), and Thiemo Voigt ([Uppsala University]).

# Dataset 
### The data collection has been performed accordingly to the following procedure:
- We adopted [Airodump-ng] to identify the victim access point and the devices connected to it. 
- Identifying information such as MAC addresses and WiFi channel used by the devices in the network.
- Setting the Alfa card channel to the one used by the smart device.
- Using either [TCPDump] or [Wireshark] for traffic collection and filtering out the traffic generated from the access point to each of the IoT device. Using the MAC address obtained from the first step.
- Extract the time and packet size associated with each over-the-air message.

### Each dataset corrosponde to the following device -- service (direct access to the RAW files):
- [Amazon Echo -- Music](https://raw.githubusercontent.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/blob/main/Amazon%20Echo%20--%20Music.txt)
- [Amazon Echo -- News](https://raw.githubusercontent.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/blob/main/Amazon%20Echo%20--%20News.txt)
- [Amazon Echo Dot -- Music](https://raw.githubusercontent.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/main/Amazon%20Echo%20Dot%20--%20Music.txt)
- [Amazon Echo Dot -- News](https://raw.githubusercontent.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/main/Amazon%20Echo%20Dot%20--%20News.txt)
- [Google Nest Mini -- Music](https://raw.githubusercontent.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/blob/main/Google%20Nest%20Mini%20--%20Music.txt)

### Each file contains the following columns:

- RAW Time: in **Seconds since beginning of capture**
- RAW Packet size: in **Bytes**

### Citing this work
When using this dataset, please make sure you cite the paper as following:

```
@article{hussain2020dark,
  title={The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services},
  author={Hussain, Ahmed Mohamed and Oligeri, Gabriele and Voigt, Thiemo},
  journal={arXiv preprint arXiv:2009.07672},
  year={2020}
}

@InProceedings{hussainIoTDark,
  author="Hussain, Ahmed Mohamed
  and Oligeri, Gabriele
  and Voigt, Thiemo",
  editor="Wang, Guojun
  and Chen, Bing
  and Li, Wei
  and Di Pietro, Roberto
  and Yan, Xuefeng
  and Han, Hao",
  title="{The Dark (and Bright) Side of IoT: Attacks and Countermeasures for Identifying Smart Home Devices and Services}",
  booktitle="Security, Privacy, and Anonymity in Computation, Communication, and Storage",
  year="2021",
  publisher="Springer International Publishing",
  address="Cham",
  pages="122--136",
  abstract="We present a new machine learning-based attack that exploits network patterns to detect the presence of smart IoT devices and running services in the   WiFi radio spectrum. We perform an extensive measurement campaign of data collection, and we build up a model describing the traffic patterns characterizing three popular IoT smart home devices, i.e., Google Nest Mini, Amazon Echo, and Amazon Echo Dot. We prove that it is possible to detect and identify with overwhelming probability their presence and the services running by the aforementioned devices in a crowded WiFi scenario. This work proves that standard encryption techniques alone are not sufficient to protect the privacy of the end-user, since the network traffic itself exposes the presence of both the device and the associated service. While more work is required to prevent non-trusted third parties to detect and identify the user's devices, we introduce Eclipse, a technique to mitigate these types of attacks, which reshapes the traffic making the identification of the devices and the associated services similar to the random classification baseline.",
  isbn="978-3-030-68884-4"
}
```

## License
[GPL-3.0](https://github.com/AMHD/The-Dark-and-Bright-Side-of-IoT-Dataset/blob/main/LICENSE)

[Uppsala University]: <https://www.it.uu.se/>
[Hamad Bin Khalifa University]: <https://www.hbku.edu.qa/en/division/information-computing-technology>
[TCPDump]: <https://www.tcpdump.org>
[Wireshark]: <https://www.wireshark.org/>
[Airodump-ng]: <https://www.aircrack-ng.org/doku.php?id=airodump-ng>
[SPIoT 2020]: <http://www.spaccs.org/spiot2020/>
[SpaCCS 2020]: <http://www.spaccs2020.com/>
[paper]: <https://arxiv.org/abs/2009.07672>
