# Bitdefender-Gen
Bitdefender-Gen - generates accounts for Bitdefender antivirus with a XX-day license

![](img/project_preview.png)

# How to use

## Using GitHub Actions CI
You can simply use the GitHub actions workflow given [here](https://github.com/rzc0d3r/ESET-KeyGen/blob/main/.github/workflows/eset.yml) in your GitHub repo.

Make a fork of my project. Go to it.
Then goto the **Actions** tab, choose **Generator** actions and then run the workflow.

It will ask the number of accounts, keys to be generated.

## Using your device

### Installing Browser
#### Google Chrome (fully supports)

1. [How to install Chrome on Windows](https://support.google.com/chrome/answer/95346?hl=en&co=GENIE.Platform%3DDesktop#zippy=%2Cwindows)
2. [How to install Chrome on Linux](https://support.google.com/chrome/answer/95346?hl=en&co=GENIE.Platform%3DDesktop#zippy=%2Clinux)
3. [How to install Chrome on Mac](https://support.google.com/chrome/answer/95346?hl=en&co=GENIE.Platform%3DDesktop#zippy=%2Clinux%2Cmac)

#### Mozilla Firefox (fully supports)
1. [How to install Firefox on Windows](https://support.mozilla.org/en-US/kb/how-install-firefox-windows)
2. [How to Install Firefox on Linux](https://support.mozilla.org/en-US/kb/install-firefox-linux)
3. [How to Install Firefox on Mac](https://support.mozilla.org/en-US/kb/how-download-and-install-firefox-mac)

#### Microsoft Edge (The project fully supports it only on Windows)
1. [Download](https://www.microsoft.com/en-us/edge/download?form=MA13L8)

### Installing python and libraries

> You can skip this step if you use the compiled executable file from the release

1. Go to the official [Python website](https://www.python.org/downloads) and download the version for your system (the project runs starting with [Python 3.8.0](https://www.python.org/downloads/release/python-380))

2. Next, install/upgrade the Python libraries, in terminal using requirements.txt:

```
pip install -r requirements.txt
```

## Preparing Bitdefender Antivirus
Delete your current Bitdefender account

## How to use (Part 2)
1. [Account Generator](wiki/AccountGenerator.md)
3. [Command Line Arguments](wiki/CommandLineArguments.md)
---

# Additional information
1. Do not minimize or close the browser window before the program is finished!!!
2. Do not create many accounts in a short period of time, otherwise you will be blocked in Bitdefender for a certain period of time
3. If the program crashes after many attempts and you know that the program is up to date. Try using a VPN
4. You can use the ``--skip-webdriver-menu`` argument, which will skip my WebDriverInstaller shell (Useful for various bugs with webdriver updates, and when using a non-standard browser like Brave or some dev-build, etc).
   The program will also install the browser itself via selenium-manager if it is not present in your system!
5. If you are having trouble initializing any web driver, I recommend manually specifying the path to the browser .exe file via ``--custom-browser-location``
