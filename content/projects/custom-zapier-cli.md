+++
date = "2022-10-22"
title = "Custom Zapier CLI - Automation Platform"
description = "A custom CLI-based automation platform inspired by Zapier, enabling seamless integration between various services."
demo_url = "https://github.com/manish001in/custom-zapier-cli"
rank = 5
+++

**A custom version of a CLI zapier, imagining how internal zapier platform might work.**

## Overview

Custom Zapier CLI is a Python-based automation platform that enables seamless integration between various services and applications. Built as a command-line interface, it demonstrates how internal automation platforms might function, providing a foundation for building custom workflow automations.

## Key Features

- 🔗 **Service Integration** - Connect multiple services like Google Apps, Dropbox, and email systems
- ⚡ **Async Processing** - Built with Celery for handling background tasks and workflows
- 🗄️ **Database Management** - PostgreSQL integration for reliable data storage
- 📊 **Google Sheets Integration** - Automated data synchronization with Google Sheets
- 📁 **Dropbox Automation** - File monitoring and automated downloads based on change detection
- 🔄 **Workflow Engine** - Core engine for managing and executing automation workflows

## Technical Architecture

- **Backend Framework:** Python with Django
- **Task Queue:** Celery for async processing
- **Database:** PostgreSQL for data persistence
- **Service APIs:** Google Apps API, Dropbox API
- **Architecture:** Modular design with separate components for each service

## Use Cases

### Primary Automation Workflows

1.**Email to Google Sheets**
   - Automatically extract data from emails
   - Create new rows in Google Sheets with email data
   - Perfect for lead tracking and data collection

2.**Dropbox File Monitoring**
   - Monitor Dropbox folders for file changes
   - Download files that have been modified within specified time duration
   - Automated file synchronization and backup

## Links

- 🌐 **GitHub Repository:** [github.com/manish001in/custom-zapier-cli](https://github.com/manish001in/custom-zapier-cli)

---

*Demonstrating how internal automation platforms can be architected for scalable workflow management.* 