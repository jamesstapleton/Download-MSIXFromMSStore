# Download-MSIXFromMSStore

This repository contains a PowerShell script designed to retrieve MSIX downloads from the Microsoft Store (MSStore) using the Microsoft Windows Update Client Web Service (WUS). This script fills the gap where WinGet package manager support for some MSStore apps is unavailable.

The recommendation is still to use WinGet's download feature for apps that do support that.

# Overview
The Download-MSIXFromStore.ps1 script connects to the Microsoft Windows Update Client Web Service (WUS) and uses SOAP-based requests to retrieve metadata and secure download URLs for MSIX or APPX applications. The script allows users to specify their target architecture (x64, x86, arm, or all) and file extension (msix, appx, or all) for precise control over what files are retrieved and downloaded.

# Key Features:
- MSStore Download Support: Bypasses the limitations of WinGet for retrieving specific MSIX files.
- Architecture-Specific Filtering: Users can filter downloads by architecture (e.g., x64, x86, arm).
- Extensive Logging and Verbose Output: Helpful logging and verbose output to aid debugging and provide insights into the script's progress.
- Versioning and Future Updates: Future improvements planned for the script are tracked and versioned, ensuring continuous enhancement.

# Prerequisites
- PowerShell 5.1 or later
- Active Internet connection to interact with Microsoft Update services
- Permissions to interact with the Windows Update Client Web Service
- Administrative permissions (recommended) for downloading and saving files
