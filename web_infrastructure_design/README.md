# Web Infrastructure Design

This project contains a series of infrastructure design diagrams and documentation for setting up a scalable, secure, and monitored web stack.

## Technologies Used

- **Linux (Ubuntu)**
- **Nginx** – Web server
- **PHP/Python/Node.js** – Application logic
- **MySQL** – Database
- **HAProxy** – Load balancer
- **SSL (Let's Encrypt)** – HTTPS encryption
- **Firewalls** – Basic iptables/ufw rules
- **Monitoring** – SumoLogic / Prometheus

## Tasks Overview

### Task 0: Simple Web Stack

- Single server with Nginx, application, and MySQL.
- Domain: `www.foobar.com` pointing to `8.8.8.8`.

### Task 1: Distributed Web Infrastructure

- Two application servers behind one HAProxy load balancer.
- Application servers contain Nginx, app logic, and a replicated MySQL setup.

### Task 2: Secured & Monitored Infrastructure

- HTTPS with SSL certificate.
- Three firewalls and three monitoring agents added.
- Monitoring system tracks QPS and server health.

### Task 3: Scale Up

- Second HAProxy for load balancer clustering.
- Separate servers for each role: web, app, DB.
- Enhanced scalability and fault tolerance.

## Acronyms

- **LAMP**: Linux, Apache (or Nginx), MySQL, PHP
- **SPOF**: Single Point of Failure
- **QPS**: Queries Per Second

## Goal

Design a web infrastructure that is:
- Redundant
- Secure
- Monitored
- Scalable

Each task includes a diagram (linked in the answer files) and explanations for all key components.