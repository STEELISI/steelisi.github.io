My name is Jelena Mirkovic and I am Research Associate Professor at University of Southern California and a PI of the [DISCERN project](../). For this project, I and my research team are running a user study on [SPHERE research infrastructure](https://sphere-testbed.net) to collect data on legitimate use of research infrastructures. The study has been reviewed and approved as exempt by the USC's Institutional Review Board (IRB). Here is more information about the study.

- **Who is running the study?**

  - Jelena Mirkovic, Research Associate Professor, USC
  - Spencer Stingley, Research Programmer, USC
  - Qishen Liang, Graduate Student Volunteer, USC

- **Why is this study being run?**
  - We need data about how legitimate users use research infrastructure, so we could build models of such use. Legiitmate use models help research infrastructures build misuse detection algorithms and catch users that run cryptomining or launch attacks using research hardware. Our study is collecting data about legitimate user's use of research infrastructure.

- **Is the study opt-in or opt-out?**
  - This is an opt-out study. All experiments ran during the study's duration (see the next question for details) will be included in data collection. If you want to opt-out, please use image names `bullseye-optout` and `2204-optout` for your experiments during the study period.

- **When, where and how is the study being run?**
  - Data collection will occur on the [SPHERE research infrastructure](https://sphere-testbed.net) from Oct 20 to Nov 20, 2025. Data will be collected by instrumenting SPHERE's `bullseye` and `2204` OS images to collect and trasmit data to a database on SPHERE.

- **What is being collected?**
   - CPU usage, memory usage, live processes, file changes and network traffic (header-only) on experimental nodes.

- **How is user privacy protected?**
  - We anonymize all data that could reveal a user's identity. Here is the list of all data collected and how it is processed:
    - Testbed node name 
    - Allocation name (chosen by user, anonymized by us)
    - Project name (chosen by user, anonymized by us)
    - Experiment name (chosen by user, anonymized by us)
    - Timestamp in Epoch time
    - CPU load (percentage 0-100)
    - File name and operation (create, delete, write), anonymized file owner and group, file hash - only for system files in the following directories: /tmp, /boot, /root, /bin, /usr, /etc
    - Network packets: timestamp, length, device (e.g. eth0, eth1), link protocol, transport protocol, network protocol, source and destination port number, source and destination IP address (both addresses have last octet anonymized)
    - System processes: process id, parent process id, memory usage, thread usage, state, user id (numeric), group id (numeric), process name 

    We anonymize necessary pieces of information by replacing strings with random other strings in a consistent manner for a given user. This approach to anonymization
requires us to keep a mapping of the original and the replacement string. After the user
ends one given experiment, we will end data collection from that experiment and we will
destroy the mapping. Another experiment by the same user will generate a new
mapping.

- **How is intellectual property protected?**
  - We do not collect any data about user's command line activities, nor any file or network packet contents.
      
- **Where can I find study's results?**
  - All results will be released on our [DISCERN project's Web page](../)

- **Who do I contact with more questions?**
  - Please email <a href="mailto:mirkovic@isi.edu">Jelena Mirkovic at mirkovic@isi.edu</a>.