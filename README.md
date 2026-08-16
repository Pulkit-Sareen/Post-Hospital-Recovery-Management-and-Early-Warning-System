# Post-Hospital Recovery Management and Early-Warning System

**UCS503P Project (2026-27 ODD)**

A web-based platform for post-hospital surgical recovery management that provides continuous monitoring, decision-support features, and early-warning indicators to healthcare professionals.

## Project Overview

This system connects patients, healthcare professionals, and recovery data through a structured workflow that:
- Allows patients to submit daily recovery information
- Monitors recovery trends and identifies unusual patterns
- Provides rule-based and ML-based alerts for professional review
- Maintains structured longitudinal recovery records
- Supports 10 common surgical recovery categories

**Team:** Pulkit Sareen, Shivam Singh, Daksh Anand (CSED)

## Project Structure

### Reports
Three reports in LaTeX format:
- **`project-proposal/`** — Project Proposal (submitted to Ms Paramveer Sidhu)
- **`project-report-prototype-stage/`** — Prototype Stage Report
- **`project-report-final/`** — Final Project Report

### Documentation & Collaboration
- **`journals/`** — Team member journals (one folder per team member)
- **`docs/`** — Project documentation in Markdown format
- **`code/`** — Source code (C++/backend and frontend)
  - `src/` — Source files
  - `inc/` — Header files
  - `Makefile` — Build configuration

### Assets
- **`assets/`** — Icons and stylesheets for documentation

## Building the Project

### Compiling the LaTeX Proposal

Install MiKTeX or TeX Live, then run:

```bash
cd project-proposal
xelatex main.tex
```

Or use VS Code with LaTeX Workshop extension.

### Local Documentation Server

To view and test documentation locally:

```bash
make docs
```

This uses [`mkdocs`](https://www.mkdocs.org/) to build and serve the documentation including team journals.

## Tech Stack

**Frontend:** React with Tailwind CSS  
**Backend:** FastAPI with Python  
**Database:** PostgreSQL or MongoDB  
**ML:** scikit-learn, NumPy, pandas  
**Deployment:** Docker, GitHub Actions (CI/CD)  
**Visualization:** Recharts

## Key Features

- **Daily Recovery Check-ins:** Patients record structured health measurements
- **Recovery Scoring:** Transparent weighted formula summarizing recovery dimensions
- **Rule-based Monitoring:** Configurable alerts for concerning patterns
- **ML-based Trajectory Analysis:** Classification (On Track, Delayed, Potentially Concerning) and anomaly detection
- **Professional Dashboard:** Priority-based patient review interface
- **Medication & Exercise Tracking:** Adherence monitoring and scheduling

## Development Phases

**Iteration 1:** Core recovery workflow (authentication, plans, daily logs, basic dashboard)  
**Iteration 2:** Recovery scoring, trends, rule-based alerts  
**Iteration 3:** ML pipeline, data generator, model training  
**Iteration 4:** Professional command center, ML visualization  
**Final:** Security, testing, performance optimization, documentation

## Resources

- **Proposal:** See `project-proposal/main.pdf` for full project details
- **Documentation:** Build with `make docs` for full documentation site
- **Journals:** Team progress tracked in `journals/


## Docs

As of now, the `docs` is just an organised collection
of markdown (`md`) files.  But the build procedure is
using [`mkdocs`](https://google.com/search?q=mkdocs)
backend.  As a result, any commit into the `master`
branch of github repository would result in CI/CD based
build and deployment of the documentation including the
journals.

For a local DEV-version of the docs for viewing and
testing, install the local env and issue the following
command:

``` shell
make docs
```

### Local `env` for `docs`

``` shell

```
