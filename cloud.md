# Cloud Services

This section evaluates the suitability of cloud services for Truelec by comparing cloud-based virtual machines with traditional on-premise servers. The organisation currently hosts all servers internally, primarily at the headquarters. However, with increasing operational scale and ageing infrastructure, cloud services are being considered as an alternative solution.

The evaluation focuses on replacing the existing servers used for the organisation’s special-purpose booking application. This analysis includes a comparison of cloud virtual machine costs from multiple cloud providers, an assessment of long-term costs over a five-year period, and a discussion of the advantages and disadvantages of cloud-based infrastructure compared to purchasing new physical servers.

---

## Cloud Server Requirements

Truelec operates a booking application that currently requires multiple servers to support its operations. Based on the project scenario, the following server requirements have been identified:

- Three servers are required at the headquarters to support the booking application and related services.
- One server is required at each branch office.
- The organisation operates three branch offices.

This results in a total requirement of six servers. These servers are currently hosted on five-year-old Dell PowerEdge Tower Servers. The organisation is considering whether to replace these servers with new on-premise hardware or migrate them to cloud-based virtual machines.

To support this decision, cloud virtual machine pricing from multiple cloud service providers is evaluated using official pricing calculators. The specifications used for comparison are kept consistent across providers to ensure a fair and accurate cost comparison.


##  Cloud Virtual Machine Configuration

To ensure a fair and consistent comparison between different cloud service providers, a standard virtual machine configuration has been selected. The same configuration is used across all cloud platforms evaluated in this project.

The selected configuration is designed to support a medium-scale booking application with moderate processing, memory, and storage requirements.

### Selected Virtual Machine Specifications

| Configuration Parameter | Selected Value |
|-------------------------|----------------|
| Region | Australia (Sydney) |
| Operating System | Ubuntu Server (Linux) |
| Virtual CPU (vCPU) | 2 vCPU |
| Memory (RAM) | 8 GB |
| Storage Type | SSD |
| Storage Size | 100 GB |
| Billing Model | Pay-as-you-go |

### Configuration Justification

- An Australian region has been selected to minimise latency and comply with data residency requirements.
- Ubuntu Server is chosen due to its stability, security, and cost-effectiveness.
- Two virtual CPUs provide sufficient processing capability for application workloads.
- Eight gigabytes of RAM supports smooth application performance and concurrent user access.
- Solid-state storage ensures faster read and write operations for application data.
- A pay-as-you-go billing model allows flexibility and avoids long-term financial commitment.
