# NSSA-320 Ansible Automation Project

## Overview

This project demonstrates an infrastructure automation solution built
using **Ansible roles**. It provisions and configures a web application
environment including Apache web servers, HAProxy load balancing,
firewall configuration, SELinux management, and automated package
updates.

------------------------------------------------------------------------

## Architecture

-   Apache Web Server
-   HAProxy Load Balancer
-   Firewall Exception Management
-   SELinux Configuration
-   Automatic System Updates using dnf-automatic

------------------------------------------------------------------------

## Project Structure

project-nssa-320-master/ 
├── main.yml 
  └── roles/ 
    ├── apache/ 
    ├── haproxy/ 
    ├── firewall_exceptions/ 
    ├── selinux/ 
    └── dnf_automatic/

------------------------------------------------------------------------

## Usage

ansible-playbook -i inventory main.yml

------------------------------------------------------------------------

## Features

-   Role-based Ansible structure
-   Idempotent infrastructure deployment
-   Automated firewall and SELinux configuration
-   Load-balanced web deployment

------------------------------------------------------------------------

## Author

NSSA Automation Project
