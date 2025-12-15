## OWASP ZAP Automated DAST

### What this does
- Runs OWASP ZAP in daemon mode
- Performs baseline or full active scan
- Enforces security gate (fail on High/Critical)
- Produces auditable artifacts

### Prerequisites
- OWASP ZAP running on :8090
- Python 3.11+
- Valid ZAP API key

### Setup
cp env.example .env
edit .env

### Usage
make baseline
make full

### Gate Logic
- High/Critical → FAIL
- Others → PASS
