## AWS Cloud Project

Quick notes to run this project.

### Get the code from GitHub
You can clone the repo or download a ZIP.

1) Clone (recommended):
```powershell
# Replace with your repository URL
git clone https://github.com/ofekh12/project-cloud.git
# Change directory into the project
cd project-cloud/aws
```

2) Download ZIP:
```powershell
# Download ZIP from GitHub (Code > Download ZIP)
# Then extract and enter the folder, for example:
Expand-Archive -Path .\project-cloud-main.zip -DestinationPath .\project-cloud
cd .\project-cloud\aws
```

### Prerequisites
- **Python**: Python 3.10+ recommended
- **AWS CLI**: Installed and configured (`aws configure`)

### Setup (Windows PowerShell)
```powershell
# From the repo root, go to the project directory
cd .\aws

# Create and activate a virtual environment
python -m venv .venv
.\.venv\Scripts\Activate.ps1

# Install dependencies
pip install -r requirements.txt
```

### AWS credentials
aws configure
```bash
# Bash (Linux/macOS): set credentials in current shell
export AWS_ACCESS_KEY_ID="YOUR_ACCESS_KEY_ID"
export AWS_SECRET_ACCESS_KEY="YOUR_SECRET_ACCESS_KEY"

```

### Run
```powershell
python PYTHONCODE.py
```

### Files
- `PYTHONCODE.py` — main script
- `requirements.txt` — Python deps
- `instancesrunning.png` — screenshot/diagram

### Quick fixes
- Credentials/AccessDenied: check IAM and region.
- Missing deps: run `pip install -r requirements.txt` inside the venv.


