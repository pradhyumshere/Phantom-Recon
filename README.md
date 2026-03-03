# Phantom Recon

### AI-Assisted Network Reconnaissance Tool

------------------------------------------------------------------------

## Overview

Phantom Recon is a Python-based reconnaissance tool that combines Nmap
scanning with AI-powered analysis using Google Gemini.

It performs structured port and service enumeration, then sends the
findings to Gemini for intelligent analysis. The AI provides
vulnerability insights, possible risk explanations, and suggested
Metasploit modules for controlled lab environments.

> This tool focuses on reconnaissance intelligence. It does not automate
> exploitation.

------------------------------------------------------------------------

## Core Purpose

Traditional scanning tools produce raw technical output that requires
manual interpretation.

Phantom Recon improves this process by:

-   Extracting important service details
-   Structuring scan results
-   Highlighting possible weaknesses
-   Suggesting relevant Metasploit modules
-   Recommending additional Nmap commands

------------------------------------------------------------------------

## Workflow

    Target Input
       ↓
    Scan Mode Selection
       ↓
    Nmap Execution
       ↓
    XML Output Generation
       ↓
    Port & Service Parsing
       ↓
    Gemini AI Analysis
       ↓
    Structured Security Report

Each stage is modular and clearly separated.

------------------------------------------------------------------------

## Features

### Scanning Engine

-   Multiple predefined scan modes
-   Interactive scan configuration wizard
-   Real-time scan progress tracking
-   XML-based result handling

### AI Analysis Module

-   Sends structured findings to Gemini
-   Generates OS and service summaries
-   Provides vulnerability insights
-   Suggests Metasploit modules
-   Recommends additional Nmap commands

### Reporting

-   Clean terminal output using rich
-   Option to export full Markdown report
-   Timestamped report files

------------------------------------------------------------------------

## Scan Modes

Phantom Recon includes both simple and advanced scanning options:

-   Stealth Scan -- SYN scan with lower timing
-   Aggressive Scan -- OS detection, version detection, scripts
-   Normal Scan -- TCP connect scan
-   Custom Builder -- Fully interactive configuration
-   Turbo Mode -- High-speed scan

### Custom Builder Allows

-   Scan technique selection
-   Port range control
-   Version detection intensity
-   OS detection
-   NSE script categories
-   Timing level adjustment
-   Basic evasion options

------------------------------------------------------------------------

## Sample Output (Lab Example)

Open Ports Detected:

-   21/tcp -- vsftpd 2.3.4
-   22/tcp -- OpenSSH 4.7p1
-   80/tcp -- Apache 2.2.8

AI Analysis May Include:

-   Service risk summary
-   Possible vulnerabilities
-   Suggested Metasploit modules
-   Additional Nmap commands for deeper testing

------------------------------------------------------------------------

## Technical Highlights

-   Built in Python
-   Uses Nmap for network scanning
-   Uses Google Gemini for AI reasoning
-   Parses XML for structured analysis
-   Clean CLI interface powered by rich
-   Modular architecture for future expansion

------------------------------------------------------------------------

## Design Principles

-   Clear separation between scanning and analysis
-   Structured data before AI processing
-   Human-readable output
-   Lab-focused usage
-   No automatic exploitation

------------------------------------------------------------------------

## Ethical Use

Phantom Recon is intended for:

-   Personal lab environments
-   Virtual machines
-   Authorized security testing

------------------------------------------------------------------------

## Project Goal

This project demonstrates:

-   Practical red team reconnaissance workflow
-   Integration of traditional security tools with AI
-   Automated intelligence from structured network data
-   Secure API handling and modular tool design
