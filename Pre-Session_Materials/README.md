# Pre-Session Instructions

## 1. Complete the [Pre-session Survey](https://forms.office.com/r/Mi4dPaDyMN)
Please complete the [survey](https://forms.office.com/r/Mi4dPaDyMN). It should only take you ~5 minutes and it will help us customize the workshop to your needs and abilities.

<br>

## 2. TVB Install, Setup, and Verification
<details>
 <summary> Click here to expand setup instructions </summary>
  
### 1. Follow Docker setup instructions 
This workshop uses a containerized software environment. Please install **Docker Desktop** on your computer prior to the workshop.

#### System Requirements
- A **64-bit** operating system  
- At least **4 GB of RAM** recommended  
- Privileges to install software  

---

#### Windows

1. Download Docker Desktop for Windows:
   - https://docs.docker.com/desktop/setup/install/windows-install/
2. Follow the on-screen installation instructions.
3. When prompted, enable **WSL 2** (Windows Subsystem for Linux).
   - Docker Desktop will guide you through this if it is not already installed.
4. Launch Docker Desktop and confirm it is running (you should see "Engine running" in the bottom left corner).

---

#### macOS

1. Download Docker Desktop for macOS:
   - https://docs.docker.com/desktop/setup/install/mac-install/
2. Choose the correct installer for your system:
   - **Apple Silicon (M1/M2/M3)** or **Intel** processor
3. Follow the on-screen installation instructions.
4. Launch Docker Desktop and confirm it is running (you should see "Engine running" in the bottom left corner).

---

#### Verify Installation

After installation, open a terminal and run:

```bash
docker --version
```

### 2. Identify or Create a tvb folder on your computer
#### Mac and Linux Users:
#### Windows Users:


### 3. Pull the Docker image
#### Mac and Linux Users:
i. Open a terminal
ii. Paste & run:
  ```docker pull lrokos/tvb_node:latest``
  
#### Windows Users:
#### All Users:
How to pull docker image and where to pull to


### 4. Start your JupyterLab Session

Open your command line 
Use the command line to start the JupyterLab session using Docker, binding to your tvb folder


### 5. Run the Installation_Test.ipynb notebook
</details>

<br>

## 3. Watch Past Recordings
Please watch these introductory videos to TVB from a similar [TVB workshop series](https://github.com/McIntosh-Lab/tvb_study_group/tree/main)
1. [**TVB Foundational Theory**](https://1sfu-my.sharepoint.com/personal/jwa415_sfu_ca/_layouts/15/stream.aspx?id=%2Fpersonal%2Fjwa415%5Fsfu%5Fca%2FDocuments%2FTVB%5Fstudy%5Fgroup%2F1%2Emov&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E90bb1e2b%2Dccac%2D467b%2D8370%2D71004d590783) - A (nearly) math-free primer on large-scale modelling in TheVirtualBrain

2. [**Post-processing Considerations**](https://1sfu-my.sharepoint.com/:v:/g/personal/jwa415_sfu_ca/EVdHkycGT_VBscB6KE7Z4F0BNmcmErMSRIpNWQ_SkF5sPQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=aA0YLz) - Imaging inputs and post-processing considerations for brain network modelling
