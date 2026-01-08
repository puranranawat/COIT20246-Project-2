# Cloud Services
This section gives pricing for a cloud setup for the company.

[Cloud VM Provider Comparison](#cloud-vm-provider-comparison) | [Total Cost](#total-cost-of-cloud-vms) | [Plan](./plan.md) | [Network Design](./network.md) | [Security](./security.md) | [Ethics](./ethics.md) | [Reflection](./reflection.md) | [Return to index](./README.md)

---

## Cloud VM Provider Comparison

This section evaluates cloud-based virtual machines as an alternative to replacing the organisation’s existing on-premise servers. Truelec currently operates its booking application on ageing physical servers hosted at the headquarters. To support future growth and reduce infrastructure management overhead, cloud virtual machines are considered.

To ensure a fair comparison, the same virtual machine configuration was used across all cloud providers. The selected configuration represents a medium-scale server suitable for the booking application workload.

### Virtual Machine Configuration Used

| Configuration Parameter | Selected Value |
|------------------------|----------------|
| Region | Australia (Sydney) |
| Operating System | Ubuntu Server (Linux) |
| vCPU | 2 vCPU |
| Memory | 8 GB |
| Storage | 100 GB SSD |
| Billing Model | Pay-as-you-go |

---

### Amazon Web Services (AWS) Pricing

Amazon Web Services (AWS) was evaluated using the official AWS Pricing Calculator. The estimate was calculated using the Asia Pacific (Sydney) region and an on-demand billing model.

| Cost Component | Details |
|----------------|---------|
| Cloud Provider | Amazon Web Services (AWS) |
| Region | Asia Pacific (Sydney) |
| Operating System | Ubuntu Server (Linux) |
| vCPU | 2 vCPU |
| Memory | 8 GB |
| Storage | 100 GB SSD |
| Billing Model | Pay-as-you-go |
| Estimated Monthly Cost (1 VM) | AUD 5,939 |

---

### Microsoft Azure Pricing

Microsoft Azure was evaluated using the official Azure Pricing Calculator. The estimate was generated using the Australia East region and a pay-as-you-go billing model. Pricing originally provided in USD was converted to AUD using an approximate exchange rate for reporting purposes.

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

---

Links to cloud provider export files:
- [AWS](./cloud/aws_vm_pricing.csv)  
- [Azure](./cloud/ExportedEstimate.xlsx)

---

## Total Cost of Cloud VMs

Based on the project scenario, Truelec requires a total of six servers to support its booking application and related services. This includes three servers at the headquarters and one server at each of the three branch offices.

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

The comparison shows that Microsoft Azure provides a lower estimated total cost over a five-year period for the selected virtual machine configuration. Based on this cost advantage, along with scalability and availability of Australian data centres, Microsoft Azure is considered the more suitable cloud service provider for Truelec.
