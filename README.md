# Windows 11 Fresh Install (CraftzCode)

This guide will walk you through setting up a fresh installation of Windows 11 for development, including updating the system, installing necessary tools, and configuring your environment.

### Set Up Windows 11
1. Update Windows 11 via **Windows Update**.
2. Update drivers using **Driver Booster**.
3. Restart your PC.
4. Repeat steps 1 and 2 to check for any remaining updates.
5. Uninstall unnecessary pre-installed apps.
6. Update your apps in the **Microsoft Store**.

### Set Up Development Tools
1. **Git**

   Install Git by running the following command:
   ```powershell
   winget install --id Git.Git -e --source winget
   ```
   Alternatively, you can download Git from their [official website](https://git-scm.com/downloads/win).

2. **Scoop**

   Install Scoop by following the instructions on the [Scoop website](https://scoop.sh/#/).
