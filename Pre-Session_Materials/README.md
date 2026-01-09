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
If successful, you should see something along the lines of `Docker version 29.1.3, build f52814d`

---

### 2. Pull the Docker image
Once Docker Desktop is installed and running, you will need to download (pull) the workshop Docker image. This image contains all required software and dependencies for the workshop.

> **Important:** Docker Desktop must be open and running before you proceed.

---
#### Windows Users:
1. Open your preferred terminal application. You may use Windows PowerShell, Command Prompt, or Windows Terminal.
2. Paste and run the following command:

```bash
docker pull lrokos/tvb_node:latest
```

#### macOS Users

1. Open a **Terminal**.
2. Paste and run the following command:

```bash
docker pull lrokos/tvb_node:latest
```


### 3. Create a tvb folder on your computer

1. Create a folder called `tvb` on your computer. You may choose to place it in your Documents folder.
2. Copy the full filepath to this `tvb` folder
   - MacOS users can right-click their `tvb` folder and then press `Copy` or `Command+C`
   - Windows users can right-click their `tvb` folder and then press `Copy as path` or `Ctrl+Shift+C`


### 4. Start your JupyterLab Session

1. While Docker Desktop is running, open your preferred terminal application (see Section 2 for instructions on which application to use) if not already open
2. Paste and run the following command, substituting `/your/tvb/path/here` with the filepath you copied in Section 3:

```bash
docker run -p 8888:8888 -v /your/tvb/path/here:/tvb_node/tvb lrokos/tvb_node:latest
```

3. Your terminal should display a message like the following. Copy either of the three paths from your terminal into your internet browser address bar (try one of the other paths if one doesn't work).

```bash
    To access the server, open this file in a browser:
        file:path.html
    Or copy and paste one of these URLs:
        http://URL
     or http://URL
```


### 5. Clone a copy of this tvb-node repository onto your computer

1. In the JupyterLab window in your internet browser, locate the navigation pane on the left side.
2. Double click the `tvb` folder to enter it.
3. Open a Terminal tab by pressing `Terminal` under the `Other` heading on the right side.
4. Running the `pwd` command should output `/tvb_node/tvb`. If not, run `cd /tvb_node/tvb`.
5. Paste and run the following command: `git clone https://github.com/INN-SFU/tvb-node.git`
6. The tvb-node repository should now exist on your local computer in the `tvb` folder!


### 6. Verify your installation with the Installation_Test.ipynb notebook

1. In the JupyerLab window, navigate inside `tvb-node` folder
2. Then enter the `Pre-Session_Materials` folder
3. Double-click `Installation_Test.ipynb` to launch the notebook.
4. Follow the instructions in the notebook to verify your installation.


### 7. Subsequent Usage

You do not need to reinstall Docker or re-clone `tvb-node` every time you want to use this container to run TVB. You just need to:

1. Launch Docker Desktop
2. Run `docker pull lrokos/tvb_node:latest` on a terminal to update the container 
3. Run `docker run -p 8888:8888 -v /your/tvb/path/here:/tvb_node/tvb lrokos/tvb_node:latest` on a terminal to launch the JupyterLab server
4. Open the JupyterLab link in a browser

</details>

<br>

## 3. Watch Past Recordings
Please watch these introductory videos to TVB from a similar [TVB workshop series](https://github.com/McIntosh-Lab/tvb_study_group/tree/main)
1. [**TVB Foundational Theory**](https://1sfu-my.sharepoint.com/personal/jwa415_sfu_ca/_layouts/15/stream.aspx?id=%2Fpersonal%2Fjwa415%5Fsfu%5Fca%2FDocuments%2FTVB%5Fstudy%5Fgroup%2F1%2Emov&nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&ga=1&referrer=StreamWebApp%2EWeb&referrerScenario=AddressBarCopied%2Eview%2E90bb1e2b%2Dccac%2D467b%2D8370%2D71004d590783) - A (nearly) math-free primer on large-scale modelling in TheVirtualBrain

2. [**Post-processing Considerations**](https://1sfu-my.sharepoint.com/:v:/g/personal/jwa415_sfu_ca/EVdHkycGT_VBscB6KE7Z4F0BNmcmErMSRIpNWQ_SkF5sPQ?nav=eyJyZWZlcnJhbEluZm8iOnsicmVmZXJyYWxBcHAiOiJPbmVEcml2ZUZvckJ1c2luZXNzIiwicmVmZXJyYWxBcHBQbGF0Zm9ybSI6IldlYiIsInJlZmVycmFsTW9kZSI6InZpZXciLCJyZWZlcnJhbFZpZXciOiJNeUZpbGVzTGlua0NvcHkifX0&e=aA0YLz) - Imaging inputs and post-processing considerations for brain network modelling
