# Splunk Log Analysis and Threat Hunting Investigation

## Overview

This project demonstrates a complete log analysis and threat hunting workflow using Splunk Enterprise. The investigation was performed on the `tutorialdata.zip` dataset and focused on identifying suspicious authentication activity, analyzing successful and failed SSH logins, investigating malicious source IP addresses, and detecting HTTP 500 web server errors.

## Objectives

The main objectives of this project were:

* Import and validate a dataset in Splunk.
* Identify available log sources and sourcetypes.
* Investigate failed SSH authentication attempts.
* Analyze successful SSH logins for a specific user (`djohnson`).
* Investigate repeated login failures from a suspicious IP address.
* Identify IPs responsible for multiple authentication failures.
* Detect and analyze HTTP 500 Internal Server Error events.

## Key Activities

* Data ingestion and validation in the `example` index.
* Sourcetype identification and log source exploration.
* SSH authentication analysis using SPL queries.
* Investigation of brute-force and password-guessing activity.
* Source IP extraction and frequency analysis.
* Web server error investigation.
* Additional threat hunting focused on the most targeted user accounts.
* Threat assessment and security recommendations based on the findings.

## Findings

The investigation revealed:

* 109,864 indexed events.
* Multiple failed SSH authentication attempts consistent with brute-force activity.
* Successful SSH sessions associated with user `djohnson`.
* Several external IP addresses responsible for a high volume of failed logins.
* Repeated targeting of privileged accounts such as `root`, `administrator`, and `admin`.
* 781 HTTP 500 Internal Server Error events within web server logs.

## Skills Demonstrated

* Splunk Enterprise
* SPL (Search Processing Language)
* Log Analysis
* Threat Hunting
* SSH Authentication Investigation
* Security Event Monitoring
* Incident Triage
* Cybersecurity Reporting

## Author

**Nouman (Javed) Nizami**
Cybersecurity Analyst  – Epicode
