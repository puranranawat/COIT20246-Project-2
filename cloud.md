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


## AWS Cloud VM Pricing

Amazon Web Services (AWS) was selected as one of the cloud service providers for evaluation due to its wide adoption, global availability, and mature infrastructure services.

The AWS Pricing Calculator was used to estimate the cost of a virtual machine based on the configuration defined in Section 4.2.2. The calculation was performed using the Australia (Sydney) region and an on-demand billing model.

### AWS Virtual Machine Cost Summary

| Cost Component | Details |
|----------------|---------|
| Cloud Provider | Amazon Web Services (AWS) |
| Region | Asia Pacific (Sydney) |
| Operating System | Ubuntu Server (Linux) |
| vCPU | 2 vCPU |
| Memory | 8 GB |
| Storage | 100 GB SSD |
| Billing Model | Pay-as-you-go |
| Estimated Monthly Cost (1 VM) | AUD 5,939  |

The pricing estimate generated using the AWS Pricing Calculator has been exported and included in the project repository for reference.

##  Azure Cloud VM Pricing

Microsoft Azure was selected as one of the cloud service providers for evaluation due to its strong enterprise presence, integration capabilities, and availability of Australian data centre regions.

The Azure Pricing Calculator was used to estimate the cost of a virtual machine based on the standard configuration defined in Section 4.2.2. The pricing was calculated using the Australia East region and a pay-as-you-go billing model to ensure a fair comparison with other cloud providers.

### Azure Virtual Machine Cost Summary

| Cost Component | Details |
|----------------|---------|
| Cloud Provider | Microsoft Azure |
| Region | Australia East |
| Operating System | Ubuntu Server (Linux) |
| vCPU | 2 vCPU |
| Memory | 8 GB |
| Storage | 100 GB SSD |
| Billing Model | Pay-as-you-go |
| Estimated Monthly Cost (1 VM) | Approx. AUD 4,650 |

The pricing estimate was generated using the official Azure Pricing Calculator and exported as an Excel file, which has been included in the project repository. The original estimate was provided in USD and has been converted to AUD using an approximate exchange rate for reporting purposes.



## Total Cloud Cost Calculation

Based on the project scenario, Truelec requires a total of six servers to support its booking application and related services. This includes three servers at the headquarters and one server at each of the three branch offices.

The following calculations present the estimated total cloud infrastructure cost over a five-year period for both AWS and Microsoft Azure.

### Total Number of Virtual Machines

- Headquarters servers: 3
- Branch office servers: 3
- Total virtual machines: 6

---

### AWS Total Cost Calculation

| Cost Item | Calculation | Estimated Cost (AUD) |
|---------|------------|----------------------|
| Monthly cost (1 VM) | As per AWS calculator | 5,939 |
| Monthly cost (6 VMs) | 5,939 × 6 | 35,634 |
| Annual cost | 35,634 × 12 | 427,608 |
| 5-year total cost | 427,608 × 5 | 2,138,040 |

---

### Azure Total Cost Calculation

| Cost Item | Calculation | Estimated Cost (AUD) |
|---------|------------|----------------------|
| Monthly cost (1 VM) | As per Azure calculator | 4,650 |
| Monthly cost (6 VMs) | 4,650 × 6 | 27,900 |
| Annual cost | 27,900 × 12 | 334,800 |
| 5-year total cost | 334,800 × 5 | 1,674,000 |

---

### Cost Comparison Summary

| Cloud Provider | Estimated 5-Year Cost (AUD) |
|---------------|-----------------------------|
| Amazon Web Services (AWS) | 2,138,040 |
| Microsoft Azure | 1,674,000 |

The comparison indicates that Microsoft Azure offers a lower estimated total cost over a five-year period for the selected virtual machine configuration.

