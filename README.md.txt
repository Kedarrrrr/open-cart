OpenCart Setup & Debugging Project
Overview

This project documents the complete setup, configuration, and debugging of an OpenCart e-commerce application in a local development environment.
The focus is not on features, but on real-world issues that occur during installation and deployment and how they were resolved systematically.

Most OpenCart demos skip this part. This project doesn’t.

Problem Statement

During OpenCart installation and initial execution, multiple critical issues were encountered:

Missing config.php and admin/config.php

Incorrect file paths after renaming folders

Permission-related errors

Application failing to load despite successful installation steps

The objective was to identify root causes, fix them properly, and ensure the project runs on a fresh setup.

What Was Done

Installed and configured OpenCart on Apache (XAMPP)

Correctly generated and placed config.php files

Fixed path mismatches caused by directory renaming

Resolved permission and visibility issues

Used error logs instead of guesswork to debug failures

Verified that the application loads correctly after fixes

Documented setup steps for reproducibility

Tech Stack

Platform: OpenCart

Backend: PHP

Database: MySQL

Server: Apache (XAMPP)

Version Control: Git & GitHub

Project Structure (Simplified)
opencart/
├── admin/
│   └── config.php
├── catalog/
├── system/
├── config.php
└── upload/

Setup Instructions

Clone the repository

git clone https:https:https://github.com/Kedarrrrr/opencart-setup-and-debugging

Move project folder to htdocs (XAMPP)

Start Apache and MySQL

Create a MySQL database

Update database credentials in:

config.php

admin/config.php

Access the application via browser

http://localhost/opencart-/

Key Learning Outcomes

OpenCart setup is fragile if paths and permissions are ignored

Most errors are configuration-related, not code-related

Logs provide answers faster than random fixes

Deployment readiness matters more than just “it works on my system”

Why This Project Matters

This project demonstrates:

Practical debugging skills

Understanding of server-side configuration

Ability to finish and stabilize a real setup

Comfort working with imperfect documentation and broken states

These are everyday problems in real projects, not classroom examples.

Future Improvements

Dockerized setup for portability

Hosting deployment (AWS / shared hosting)

Basic automation for environment setup

Author

Kedar Gaikwad
Entry-level Software / QA Engineer
Focused on execution, debugging, and system understanding