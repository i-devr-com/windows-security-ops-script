# Windows Security Operations Automation Script

Automates forensic investigation, threat eradication, system hardening, and privacy fortification on Windows systems. Provides real-time progress bars for visibility throughout each security stage.

## Features

- Full forensic sweep: WMI, scheduled tasks, services, startup registry, users, event logs & more
- Finds and eradicates common persistence and backdoor mechanisms
- Applies Windows updates, hardens system policies, enforces encryption
- Enhances privacy and security settings for future use
- Visual loading bar shows progress at every stage

## Prerequisites

- **Windows 10/11 or Server (Admin rights required)**
- **PowerShell 5.1 or later**
- Internet connection (for module installations and updates)
- (Optional) BitLocker-compatible hardware for encryption steps

## Usage

1. **Clone or download this repository**  
git clone https://github.com/i-devr-com/windows-security-ops-script
cd windows-security-ops-script

2. **Review the script**  
- Open `SecOps-Automation.ps1` in an editor
- (Optional) Edit removal/disabling sections as needed for your environment

3. **Open PowerShell as Administrator**

4. **Run the script**
   Set-ExecutionPolicy RemoteSigned
.\SecOps-Automation.ps1


> You will see a real-time progress bar for each major security stage. Execution may take several minutes depending on system state.

5. **Review All Outputs**
- Collected artifacts and analysis results are saved as text files in the current directory
- Review these for manual follow-up or incident response as appropriate

## Notes

- **Customization highly recommended:**  
The removal/eradication section is template-based—adapt to match known bad artifacts/processes after performing initial detection.  
- **Restoration & hardening actions may cause reboots or service interruptions.**  
- **BitLocker:**  
Activating encryption will require a reboot. Back up your recovery key.  
- **Test in a lab before deploying on production or business-critical systems.**

## License

[MIT](LICENSE)

## Contributions

Open to PRs and community feedback!  
Raise issues or improvements via GitHub Issues.

---

**Stay safe, stay secured.**  
