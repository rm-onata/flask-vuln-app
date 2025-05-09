# Web Vulnerabilities with Flask

Welcome to the **Web Vulnerabilities with Flask** repository! This project showcases various web vulnerabilities and their implementations using the Flask framework. It serves as an educational resource for developers and security enthusiasts to understand common security flaws in web applications.

## Table of Contents

- [Introduction](#introduction)
- [Vulnerabilities Covered](#vulnerabilities-covered)
- [Getting Started](#getting-started)

## Introduction

Web applications are often targets for various types of attacks. Understanding these vulnerabilities is crucial for building secure applications. This repository provides practical examples of common web vulnerabilities, including:

- CSS Injection
- Cross-Site Request Forgery (OSRF)
- Open Redirect
- Server-Side Template Injection (SSTI)
- SQL Injection


Each example is implemented using Flask, a lightweight WSGI web application framework in Python.

## Vulnerabilities Covered

1. **CSS Injection**: Demonstrates how attackers can inject malicious CSS into a web application, potentially altering the appearance and behavior of the site.
2. **Cross-Site Request Forgery (OSRF)**: Illustrates how unauthorized commands can be transmitted from a user that the web application trusts, leading to unintended actions.
3. **Open Redirect**: Shows how attackers can manipulate URLs to redirect users to malicious sites, potentially leading to phishing attacks.
4. **Server-Side Template Injection (SSTI)**: Explains how attackers can inject malicious code into server-side templates, allowing them to execute arbitrary code on the server.
5. **SQL Injection**: Demonstrates how attackers can manipulate SQL queries to gain unauthorized access to data.


## Getting Started

To get a local copy of this project up and running, follow these steps:

1. **Clone the repository**:
   ```bash
   git clone https://github.com/rm-onata/flask-vuln-app
   cd web-vulnerabilities-flask
