# PDQ Registry Scanners & Deploy Packages

This repository contains PDQ Inventory scanners (Registry and PowerShell) and PDQ Deploy packages to modify or fix specific registry keys on Windows machines.

## Structure

- **PDQInventory**
  - **RegistryScanners**: `.xml` exports of registry-based scanners
  - **PowerShellScanners**: `.xml` exports of PowerShell-based scanners
- **PDQDeploy**
  - **Packages**: `.xml` exports of deployment packages
    - **RegistryFixes**: Deployment packages for fixing registry keys
    - **scripts**: PowerShell scripts called by the deployment packages
- **docs**: Additional documentation.

## Usage

1. **Import Inventory Scanner**  
   - In PDQ Inventory, go to **File** > **Import**, select the `.xml` file from `PDQInventory/RegistryScanners` or `PDQInventory/PowerShellScanners`.
   - After importing, run or schedule the scanner on target computers.

2. **Import PDQ Deploy Package**  
   - In PDQ Deploy, go to **File** > **Import**, select the `.xml` file from `PDQDeploy/Packages`.
   - Review package steps and scripts (especially file paths for `.ps1` scripts).
   - Deploy to target computers as needed.

## Contributing

1. Fork the repository.
2. Create a feature branch.
3. Commit and push changes.
4. Create a pull request to merge your changes into the main branch.

## License

[MIT License](LICENSE) - feel free to use and modify as needed.
