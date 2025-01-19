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

3. **Node.js (LTS version)**

   Install Node.js using Scoop:
   ```powershell
   scoop install nodejs-lts
   ```

4. **Nerd Fonts**

   Add the Nerd Fonts bucket and install the Hack NF Mono font:
   ```powershell
   scoop bucket add nerd-fonts
   scoop install Hack-NF-Mono
   ```

5. **Windows Terminal**

   Configure Windows Terminal to your preferences.

6. **Oh My Posh**

   Install Oh My Posh with the following command:
   ```powershell
   scoop install oh-my-posh
   ```

7. **Terminal Icons**

   Install Terminal Icons:
   ```powershell
   scoop bucket add extras
   scoop install terminal-icons
   ```

8. **Zoxide**

   Install Zoxide for smarter directory navigation:
   ```powershell
   scoop install zoxide
   ```

9. **Eza**

    Install Eza, a modern replacement for `ls`:
   ```powershell
   scoop install eza
   ```

10. **FZF**

    Install FZF for fuzzy searching:
    ```powershell
    scoop install fzf
    ```

11. **PSFZF**

    Install PSFZF for integrating FZF with PowerShell:
    ```powershell
    scoop install psfzf
    ```

12. **Set PowerShell Configuration Path**

    Set your default PowerShell profile configuration by editing `$PROFILE`:
    ```powershell
    New-Item -Path $PROFILE -ItemType File -Force
    notepad $PROFILE
    ```

    Add the following line to the file:
    ```powershell
    . $env:USERPROFILE\.config\powershell\user_profile.ps1
    ```

13. **Copy Configuration Files**

    Copy all configuration files from the `.config` folder to your local system.

14. **Visual Studio Code**

    Install VSCode by adding the extras bucket and then installing:
    ```powershell
    scoop install vscode
    ```

    Sign in to VSCode using your GitHub account to sync all your settings.

15. **Bun**

    Install Bun using Scoop:
    ```powershell
    scoop install bun
    ```

16. **Wezterm (Optional)**

    [Wezterm](https://wezfurlong.org/wezterm/installation.html)

    Create Wezterm Config File
    ```shell
    mkdir -p ~/.config/wezterm
    nano ~/.config/wezterm/wezterm.lua
    ```

    Copy my wezterm.lua

    Exit and Re-run Wezterm
