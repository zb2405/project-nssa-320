# NSSA-320 Ansible & AWX Infrastructure Automation

## Project Overview

This project demonstrates an **Infrastructure as Code (IaC)** automation
solution built using **Ansible roles** and executed through **Ansible
AWX**. The automation provisions and configures a load‑balanced web
application environment while showcasing centralized job execution,
inventory management, and GUI‑based orchestration.

The goal of the project was to reduce manual system configuration,
improve repeatability, and demonstrate enterprise‑style automation
workflows using open‑source tools.

------------------------------------------------------------------------

## Architecture

The automated environment includes:

-   Apache Web Servers
-   HAProxy Load Balancer
-   Firewall Exception Management
-   SELinux Configuration
-   Automatic Updates using `dnf-automatic`
-   Ansible AWX for centralized orchestration

------------------------------------------------------------------------

## Key Features

-   Role‑based Ansible architecture
-   GUI automation using AWX
-   Inventory and credential management
-   Idempotent configuration management
-   Automated patching and firewall configuration
-   Load‑balanced web deployment

------------------------------------------------------------------------

## Project Structure
```
    project-nssa-320-master/
    ├── main.yml
    └── roles/
        ├── apache/
        │   ├── tasks/
        │   └── files/
        │
        ├── haproxy/
        │   ├── tasks/
        │   └── files/
        │
        ├── firewall_exceptions/
        │   ├── tasks/
        │   └── handlers/
        │
        ├── selinux/
        │   └── tasks/
        │
        └── dnf_automatic/
            ├── defaults/
            ├── tasks/
            └── templates/
```
------------------------------------------------------------------------

## Usage

Run playbook manually:

``` bash
ansible-playbook -i inventory main.yml
```

Or execute through AWX by creating a job template and launching the
automation workflow.

------------------------------------------------------------------------

## Results

The automation successfully deployed the web application across all web
servers and enabled access through the load balancer. AWX provided
centralized logging, execution visibility, and simplified infrastructure
management.

------------------------------------------------------------------------

## Author

Zaki Bawade\
RIT NSSA Infrastructure Automation Project
