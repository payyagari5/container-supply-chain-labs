# container-supply-chain-labs

Lab environments and code samples for the **Chain of Custody** series on Medium — a practitioner's guide to securing the container software supply chain.

## Series articles

- [Chain of Custody: The Dependency You Didn't Know You Had Was the One That Got You](https://medium.com/@payyagari05)
- Chain of Custody: The Packages You Didn't Install *(coming soon)*

## Labs

### sc01-sbom-and-scanning

Demonstrates SBOM generation with Syft and vulnerability scanning with Trivy against a deliberately vulnerable image.

**Vulnerable image:** `python:3.8.0` with old Flask, Requests, Jinja2, and Werkzeug versions — used to demonstrate real HIGH and CRITICAL findings in CI.

**What this lab covers:**
- Generating a CycloneDX SBOM with Syft
- Scanning an image with Trivy
- Trivy config scan against Kubernetes manifests
- GitHub Actions workflow that fails a PR on CRITICAL/HIGH fixable findings

## Disclaimer

The Dockerfile and dependencies in this repo are **deliberately vulnerable** for educational purposes. Do not use in production.

## Author

Prathyusha Ayyagari — [Medium](https://medium.com/@payyagari05) · [LinkedIn](https://www.linkedin.com/in/prathyusha-ayyagari)
