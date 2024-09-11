# GCP VM Terraform Module

This Terraform module creates a simple Virtual Machine (VM) instance in Google Cloud Platform (GCP).

## Features

- Creates a single VM instance in GCP
- Uses the Debian 11 operating system
- Attaches an ephemeral public IP
- Includes a basic startup script
- Applies "web" and "dev" tags to the instance

## Prerequisites

- Terraform v0.14+ installed
- Google Cloud SDK installed and configured
- A GCP project with necessary APIs enabled (Compute Engine API)

## Usage

1. Clone this repository or copy the Terraform files to your local machine.

2. Create a `terraform.tfvars` file in the same directory with the following content:

   ```hcl
   project_id = "your-gcp-project-id"
   region     = "desired-region"  # Optional, defaults to us-central1
