# GCP Network with Terraform

A simple Google Cloud network built with Terraform (Infrastructure as Code).

## What it does
- Creates a custom VPC network named `mynetwork` (auto-created subnets in every region)
- Adds a firewall rule allowing SSH (22), HTTP (80), RDP (3389) and ICMP (ping)

## Files
- `main.tf` - provider and base configuration
- `variables.tf` - input variables
- `mynetwork.tf` - the VPC network and firewall rule

## Tools
- Terraform
- Google Cloud Platform (GCP)

## How to run
## clean up 
## Security note
The firewall rule uses `0.0.0.0/0` (open to the internet) for learning purposes.
In production, restrict `source_ranges` to specific IP addresses.
