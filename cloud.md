# Task 4.2 – Cloud Services

## 1. Cloud Requirement Summary
Truelec runs a booking application that needs reliable servers. The headquarters needs three application servers. Each branch office needs one application server. The goal is to compare cloud pricing and recommend the best cloud provider for Truelec.

## 2. Cloud Providers Considered
We compared the following cloud providers:
- Provider 1: Amazon Web Services (AWS)
- Provider 2: Microsoft Azure
- Provider 3 (optional): Google Cloud Platform (GCP)

## 3. VM Specification Assumptions
To make the comparison fair, we used the same VM specifications for all providers:
- Operating system: Linux / Windows (<<SELECT_ONE>>)
- vCPU: <<VCPU>>
- RAM: <<RAM>>
- Storage: <<STORAGE>> GB SSD
- Region: <<REGION>>
- Uptime: 24/7 usage
- Network traffic: standard business usage

## 4. Pricing and Estimates

### 4.1 AWS Estimate
- Calculator used: AWS Pricing Calculator
- Service used: EC2 virtual machine
- Export file saved as: cloud_estimates/AWS_Estimate.pdf
- Estimated monthly cost: <<MONTHLY_AWS>>
- Estimated yearly cost: <<YEARLY_AWS>>
- Estimated 5-year cost: <<FIVE_YEAR_AWS>>

### 4.2 Azure Estimate
- Calculator used: Azure Pricing Calculator
- Service used: Azure Virtual Machines
- Export file saved as: cloud_estimates/Azure_Estimate.pdf
- Estimated monthly cost: <<MONTHLY_AZURE>>
- Estimated yearly cost: <<YEARLY_AZURE>>
- Estimated 5-year cost: <<FIVE_YEAR_AZURE>>

### 4.3 GCP Estimate (Optional)
- Calculator used: Google Cloud Pricing Calculator
- Service used: Compute Engine
- Export file saved as: cloud_estimates/GCP_Estimate.pdf
- Estimated monthly cost: <<MONTHLY_GCP>>
- Estimated yearly cost: <<YEARLY_GCP>>
- Estimated 5-year cost: <<FIVE_YEAR_GCP>>

## 5. Total 5-Year Cost (All VMs)
The total number of servers required is:
- HQ: 3 servers
- Branches: 1 server per branch × <<NUMBER_OF_BRANCHES>> branches
- Total servers: <<TOTAL_SERVERS>>

The total 5-year cost is:
- AWS total 5-year cost: <<AWS_TOTAL_5_YEAR>>
- Azure total 5-year cost: <<AZURE_TOTAL_5_YEAR>>
- GCP total 5-year cost (optional): <<GCP_TOTAL_5_YEAR>>

## 6. Cloud vs On-Premise Server Purchase

### 6.1 Advantages of Cloud
Cloud hosting has several benefits:
- It is easy to scale up when business grows.
- Maintenance is handled by the cloud provider.
- High availability is possible.
- Quick deployment of servers.

### 6.2 Disadvantages of Cloud
Cloud hosting also has some drawbacks:
- Continuous monthly costs.
- Dependence on internet connectivity.
- Data security must be managed properly.

### 6.3 Advantages of On-Premise Servers
Buying physical servers has benefits such as:
- Full control of hardware and data storage.
- No monthly cloud billing.
- Can work even with limited internet.

### 6.4 Disadvantages of On-Premise Servers
On-premise servers have disadvantages such as:
- High upfront cost.
- Maintenance and upgrades are required.
- Hardware failures can cause downtime.

## 7. Final Recommendation
Based on our pricing comparison and service features, we recommend using <<RECOMMENDED_PROVIDER>>. This provider offers better pricing over 5 years and provides good reliability, security services, and scalability. It is suitable for hosting the booking application servers for HQ and branch offices.

## 8. Conclusion
In conclusion, cloud hosting is a strong option for Truelec because it provides scalable and reliable server hosting. The recommended provider offers the best overall value and support for Truelec’s booking application needs.
