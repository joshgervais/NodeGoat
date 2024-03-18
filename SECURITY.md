
# Security Policy for NodeGoat

## Supported Versions

The following table provides an overview of which versions of NodeGoat are currently receiving security updates:

| Version | Supported          |
|---------|--------------------|
| 1.3.0   | :white_check_mark: |
| < 1.3.0 | :x:                |

## Reporting a Vulnerability

We take the security of NodeGoat seriously, even though it's designed to be an insecure application for educational purposes. If you have discovered a potential security vulnerability in NodeGoat, please follow these steps to report it:

1. Open an issue in the NodeGoat repository, providing all the details about the vulnerability without disclosing sensitive information.
2. Describe the issue in detail, including the potential impact and steps to reproduce it if possible.
3. Indicate the version of NodeGoat you were using (e.g., 1.3.0).
4. Avoid disclosing the vulnerability publicly until we have had the opportunity to investigate and address the issue.

Our team will review your report and respond as soon as possible with next steps.

## Known Security Issues

In version 1.3.0, we have identified a high-severity security vulnerability related to arbitrary code execution due to unsafe handling of user input:

- Arbitrary Code Execution via `eval()` with User-Controlled Input - An attacker could exploit this by sending crafted input to the `eval()` function, leading to arbitrary code execution. We recommend refraining from using `eval()` with user-controlled data and implementing proper input validation. This issue does not have a CVE assigned but is a well-understood security risk associated with the use of `eval()`. The CVSS score is 8.8, indicating high severity.

## Security Update Policy

When a new security vulnerability is reported, we will assess the report and determine the potential impact on the NodeGoat project. If necessary, we will release updates or patches to address the issue.

We encourage all users to keep their instances of NodeGoat up-to-date with the latest security updates provided.

Thank you for helping us keep NodeGoat and its community safe!
