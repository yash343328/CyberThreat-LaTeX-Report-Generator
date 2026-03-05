# CyberThreat-LaTeX Report Generator

A **LaTeX-based Cybersecurity Incident Report Generator** that automatically creates professional threat intelligence reports with structured sections, attack diagrams, and mitigation strategies.

This project demonstrates how **LaTeX automation can be used to generate structured cybersecurity reports similar to those used by SOC (Security Operations Center) teams and incident response professionals.**

---

## Project Overview

Modern organizations generate detailed **incident response reports** after detecting cybersecurity threats.
This project provides a **custom LaTeX framework** that allows users to quickly generate those reports using simple commands.

Instead of manually formatting documents, analysts can write:

```
\newthreat{Phishing Attack}{High}{Credential Theft}{Immediate password reset required}
```

The system automatically produces a **professionally formatted threat report**.

---

## Features

* Automated **Threat Overview** sections
* Structured **Attack Timeline** documentation
* **Indicators of Compromise (IOC)** tables
* **Mitigation strategy** blocks
* **Attack path diagrams** using TikZ
* Clean **SOC-style incident report formatting**
* Modular architecture using custom **LaTeX package (.sty)**

---

## Project Structure

```
cyberthreat-latex/
│
├── main.tex                # Main report document
├── cybercommands.sty       # Custom LaTeX commands
├── sample-report.tex       # Example threat report
└── README.md
```

---

## Example Commands

### Create a Threat Report

```
\newthreat
{Phishing Attack}
{High}
{User credentials compromised}
{Enable multi-factor authentication}
```

---

### Add an Attack Timeline

```
\attacktimeline
{March 1 2026}
{Suspicious Email}
{A phishing email was sent to employees}
```

---

### Indicators of Compromise Table

```
\iocTable{
malicious-login.com & Phishing domain \\ \hline
185.92.220.14 & Suspicious login IP \\ \hline
}
```

---

## Output

After compiling the document, the generated PDF includes:

* Executive Summary
* Threat Overview
* Attack Timeline
* Indicators of Compromise
* Attack Path Diagram
* Mitigation Strategies

The result is a **professional cybersecurity incident report**.

📄 **Sample Generated Report:**
[Download cyberthreat-latex.pdf](cyberthreat-latex.pdf)

This PDF demonstrates how the system automatically formats a structured cybersecurity incident report using custom LaTeX commands.

---

## Compilation

Compile using **pdflatex**:

```
pdflatex main.tex
```

Or upload the project to **Overleaf** and click **Recompile**.

---

## Technologies Used

* LaTeX
* TikZ (for attack diagrams)
* tcolorbox (for styled report sections)
* longtable (for IOC tables)

---

## Use Cases

This system can be used for:

* Cybersecurity research documentation
* Incident response reports
* Threat intelligence documentation
* Security training material
* Academic cybersecurity projects

---

## Future Improvements

Possible upgrades for the project:

* MITRE ATT&CK framework integration
* CVSS risk scoring automation
* Threat heatmap visualization
* Multi-incident report generation
* AI-assisted threat documentation

---

## Author

**Yash Jain**

---

## License

This project is open-source and available under the **MIT License**.

---

⭐ If you found this project useful, consider giving it a star on GitHub.
