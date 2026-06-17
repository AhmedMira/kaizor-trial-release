# CyberSec Trial (Windows) — Customer Guide

This repository contains **distribution-only artifacts** for the CyberSec Trial.
It intentionally contains **no source code**.

## What this Trial is

This Trial lets you evaluate **one Kaizor capability**: a local vulnerability management workflow (assets → scans → findings → report).

Trial duration: **48 hours** (starts at activation time).

## Step-by-step (recommended)

### 1) Download
- Download `cybersec-trial-setup.exe`
- (Optional) Verify file integrity using `cybersec-trial-setup.exe.sha256`

### 2) Install
1. Run `cybersec-trial-setup.exe`
2. Finish the installer

### 3) Launch
1. Open **CyberSec Trial** from Desktop or Start Menu
2. The app will open in your browser automatically

If the browser does not open automatically:
- Open your browser and go to: `http://127.0.0.1:8080/`

### 4) Activate
1. Enter your email
2. Enter the Trial Key from `TRIAL_KEY.txt`
3. Continue to registration

### 5) Register and login
1. Create an account (email + password)
2. Log in

### 6) Add an asset
1. Go to **Assets**
2. Add an asset (IP / hostname / domain)

### 7) Upload scans
1. Go to **Uploads**
2. Upload a scan file (supported trial inputs include formats such as Nessus and Nmap XML)

### 8) Review findings
1. Go to **Findings**
2. Review findings and update status (e.g., Open → In Progress → Fixed / Accepted Risk / False Positive)

### 9) Open the report
1. Go to **Report**
2. Open the latest report view

## Troubleshooting (common)

### The app does not open in the browser
- Open your browser and go to `http://127.0.0.1:8080/`

### “Address already in use” or the page won’t load
- Close any older CyberSec Trial windows
- Restart your PC, then launch again

### Activation fails
- Double-check the Trial Key in `TRIAL_KEY.txt`
- Make sure you are connected to the internet during activation

### Upload fails
- Try uploading one file at a time
- If the file is very large, try a smaller sample for evaluation

## Support

If you run into an issue, please send:
- A screenshot of the error
- What step you were on (e.g., “Activation”, “Upload”, “Findings”)

## Kaizor Platform (separate docs)

For full Kaizor Platform documentation (capabilities, real-world problems, and diagrams), see:
- `KAIZOR_PLATFORM_README.md`
