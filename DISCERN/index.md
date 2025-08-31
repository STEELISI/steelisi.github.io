# CICI: RSSD: DISCERN: Datasets to Illuminate Suspicious Computations on Engineering Research Networks

**Project members:** Jelena Mirkovic, Brian Kocoloski, Spencer Stingley, Quishen Sam Liang, Muskan Fatima

**Funding acknowledgment:** This research is supported by the National Science Foundation's CICI program, under the award number 2319864.

Reconfigurable compute and network testbeds form the basis of much scientific cyberinfrastructure (CI). In such CI, users are given unrestricted access to experimental nodes, which can reach into the Internet and host publicly reachable services. A unifying theme across this type of CI is a desire to remain open and flexible to meet the ever evolving needs of the science and engineering communities. Yet, this openness and flexibility, coupled with a lack of system administration knowledge among CI users, opens the CI to attacks and misuse by external actors. Compromised nodes can be used to attack other public targets, they can encrypt or exfiltrate users' scientific data, or they can perform illicit computational activities such as cryptocurrency mining.

DISCERN project collects datasets that capture legitimate and illegitimate use of scientific CI, and thus can be used by cybersecurity researchers to develop detection and defense approaches for CI attacks and misuse. We have instrumented the [SPHERE research infrastructure](https://sphere-project.net) (used for cybersecurity and networking experimentation) to collect data about user activities via various user interfaces, experimental node processes, system events and file changes, experimental node resource usage and internal and external network traffic interacting with user experiments. Data is collected in a privacy-preserving and an intellectual-property-preserving manner to protect users and their research. We have further launched carefully designed, ethical attacks that misuse SPHERE nodes in a variety of realistic CI misuse scenarios, and have collected data from these events. Legitimate and illegitimate use datasets are released in their entirety, but they are also curated for diversity, interleaved to create mixed, balanced datasets, and released in that form to aid cybersecurity researchers in data mining and classification tasks. Our data collection tools and methodology are portable to other scientific CIs. We are working closely with owners of these CIs to promote their adoption of our tools and help them produce their own CI-usage datasets.

## Intellectual Merit

Our work creates new datasets capturing the way users leverage cyberinfrastructure (CI) resources to conduct scientific experiments in cybersecurity and networking. Our datasets also capture records of illegitimate use of CI. Jointly, these datasets provide resources for cybersecurity researchers to develop detection and defense approaches to protect scientific CI against misuse. Our data collection tools and methodology demonstrate how to collect realistic, rich datasets of legitimate and illegitimate CI use in a safe and ethical manner. Our approaches can be replicated by others to study different scientific CIs.

## Broader Impacts

Our proposed effort can improve cybersecurity posture of scientific cyberinfrastructure (CI) by providing realistic and diverse datasets to cybersecurity researchers, which can then work to develop appropriate defenses for CI. An improved cybersecurity posture of scientific CI in turn protects our nation's progress in science and technology by protecting privacy and intellectual property of the researchers interacting with the CI.
Our datasets are also useful for cybersecurity education, as they are fully labeled, rich and diverse. Our instrumentation efforts help track data provenance, which can improve experiment reproducibility on scientific CIs.

## Outcomes

* [Interviews with CI leaders](https://docs.google.com/document/d/1JsOU073bmc24w_9QMPQY-oMHlg-nKWleRrfS_wClmAk/edit?usp=sharing)
* [Datasets with synthetic legitimate and attack traffic](https://github.com/STEELISI/discern_data/tree/main/synthetic)
* [Code for data collection](https://gitlab.com/mergetb/tech/instrumentation)
* Technical report