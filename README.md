<a id="readme-top"></a>

<div align="center">
  <a href="https://github.com/kan08306">
    <img src="./app/Views/folder_template/assets/KBlogo.png" alt="KB Logo" width="130">
  </a>

  <h1>Web System Technologies Activities</h1>

  <p>
    A semester portfolio of my CodeIgniter 4 activities, exercises, and projects.
  </p>

  <p>
    <a href="https://github.com/kan08306/bautista_tc32"><strong>View Repository</strong></a>
  </p>
</div>

---

## Table of Contents

- [Overview](#overview)
- [Activities](#activities)
- [Technology](#technology)
- [Project Structure](#project-structure)
- [Local Installation](#local-installation)
- [Running the Project](#running-the-project)
- [Development Guidelines](#development-guidelines)
- [Resources](#resources)

## Overview

This repository contains my activities for **Web System Technologies**. It uses CodeIgniter 4 and follows the Model-View-Controller (MVC) architecture.

The project will serve as a central portfolio throughout the semester. Each activity has its own route, controller, view folder, and related assets when needed.

## Activities

| Activity | Description | Local Route | Source Code |
|---|---|---|---|
| Folder Template | Initial CodeIgniter view and routing exercise | `/folder-template` | [View files](./app/Views/folder_template/) |
| Activity 2 | To be added | `/activity2` | To be added |
| Activity 3 | To be added | `/activity3` | To be added |

> CodeIgniter uses PHP and must run on a PHP server. The local routes work after starting the development server. GitHub stores the source code but does not execute the PHP application through GitHub Pages.

## Technology

![PHP](https://img.shields.io/badge/PHP-777BB4?style=for-the-badge&logo=php&logoColor=white)
![CodeIgniter](https://img.shields.io/badge/CodeIgniter-EF4223?style=for-the-badge&logo=codeigniter&logoColor=white)
![HTML](https://img.shields.io/badge/HTML-E34F26?style=for-the-badge&logo=html5&logoColor=white)
![CSS](https://img.shields.io/badge/CSS-1572B6?style=for-the-badge&logo=css3&logoColor=white)
![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=for-the-badge&logo=javascript&logoColor=black)
![Composer](https://img.shields.io/badge/Composer-885630?style=for-the-badge&logo=composer&logoColor=white)
![Git](https://img.shields.io/badge/Git-F05032?style=for-the-badge&logo=git&logoColor=white)
![GitHub](https://img.shields.io/badge/GitHub-181717?style=for-the-badge&logo=github&logoColor=white)

## Project Structure

```text
bautista_tc32/
├── app/
│   ├── Config/
│   │   └── Routes.php
│   ├── Controllers/
│   │   └── FolderTemplate.php
│   ├── Models/
│   └── Views/
│       └── folder_template/
│           └── index.php
├── public/
│   ├── assets/
│   │   ├── css/
│   │   ├── images/
│   │   └── js/
│   └── index.php
├── writable/
├── composer.json
├── composer.lock
└── spark
```

### File locations

| Content | Location |
|---|---|
| Page templates | `app/Views/` |
| Request-handling code | `app/Controllers/` |
| Database models | `app/Models/` |
| URL routes | `app/Config/Routes.php` |
| CSS | `public/assets/css/` |
| JavaScript | `public/assets/js/` |
| Images | `public/assets/images/` |

## Local Installation

### Requirements

- PHP 8.2 or newer
- Composer 2
- XAMPP or another PHP environment
- Enabled PHP extensions: `curl`, `gd`, `intl`, `mbstring`, and `zip`

Clone the repository:

```bash
git clone https://github.com/kan08306/bautista_tc32.git
cd bautista_tc32
```

Install the Composer dependencies:

```bash
composer install
```

Create the local environment file:

```powershell
Copy-Item env .env
```

Configure `.env` for local development:

```ini
CI_ENVIRONMENT = development
app.baseURL = 'http://localhost:8080/'
```

> The `.env` file and local credentials must not be committed to GitHub.

## Running the Project

Start the CodeIgniter development server:

```bash
php spark serve
```

Open the application at:

```text
http://localhost:8080/
```

Example activity:

```text
http://localhost:8080/folder-template
```

Stop the server by pressing `Ctrl+C` in the terminal.

## Development Guidelines

- Follow CodeIgniter's MVC structure.
- Create views under `app/Views/`.
- Use controllers to load views and handle requests.
- Register activity URLs in `app/Config/Routes.php`.
- Store browser-accessible assets under `public/assets/`.
- Keep one central `public/index.php`; do not create another one for each activity.
- Do not commit `.env`, credentials, logs, cache data, or the `vendor/` directory.
- Test activities locally before committing and pushing changes.
- Update the Activities table whenever a new activity is added.

## Resources

| Resource | Purpose | Link |
|---|---|---|
| Repository | Semester source-code portfolio | [bautista_tc32](https://github.com/kan08306/bautista_tc32) |
| CodeIgniter User Guide | Framework documentation | [CodeIgniter 4 User Guide](https://codeigniter.com/user_guide/) |
| Composer | PHP dependency management | [Composer](https://getcomposer.org/) |
| PHP Manual | PHP language documentation | [PHP Manual](https://www.php.net/manual/en/) |

<p align="right"><a href="#readme-top">Back to top</a></p>
