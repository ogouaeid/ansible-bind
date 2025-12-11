# Ansible Bind DNS Automation Role

This project contains an Ansible role to automate the installation and configuration of a Master/Slave BIND DNS infrastructure, including zone file generation, service configuration, validation, and functional testing using `dig`.

## 🚀 Features

- Install BIND DNS server (master/slave)
- Configure named.conf and zone files dynamically
- DNS zone validation (`named-checkconf`, `named-checkzone`)
- Automatic firewall configuration
- Functional DNS tests via `dig`
- Support forward + reverse zones
- Idempotent and reusable

---

## 📦 Requirements

- Ansible ≥ 2.12
- Linux target hosts (CentOS, Redhat, Rocky, etc.)
- Python installed on managed nodes (unless using `raw` for bootstrap)

---

## 📁 Inputs

The role expects two variables: `servers` and `zones`.

You must create your own files based on the provided templates:



