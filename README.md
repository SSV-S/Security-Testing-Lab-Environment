# Security Testing Lab Environment

This repository documents the setup of isolated Windows security testing environments using Windows Sandbox and Oracle VirtualBox. The goal is to test applications, browser activity, and security tools without affecting the host operating system.

## Project Scope

| Environment | Purpose |
| --- | --- |
| Windows Sandbox | Temporary, disposable testing environment |
| Oracle VirtualBox | Persistent virtual lab environment |
| Windows 10 guest VM | Host/application security testing |
| VirtualBox Extension Pack | Adds support for enhanced VM features |

## Why Isolation Matters

Security testing should be performed in an isolated environment so unknown files, browser activity, configuration changes, or application behavior do not affect the primary workstation. Sandboxes and VMs help reduce risk while allowing hands-on analysis.

## Windows Sandbox Review

Windows Sandbox provides a lightweight disposable Windows environment. Any changes made inside the sandbox are discarded after it closes, making it useful for quick tests and temporary application review.

Key validation points:

- Virtualization support enabled on the host.
- Windows Sandbox feature enabled.
- Sandbox launches as a separate clean Windows environment.
- Installed software does not persist after the sandbox is closed.

## VirtualBox Lab Build

The VirtualBox portion of the project created a persistent Windows 10 VM for repeatable security testing.

Implementation highlights:

- Downloaded and installed Oracle VirtualBox.
- Installed VirtualBox Extension Pack.
- Created a Windows 10 virtual machine.
- Allocated memory and virtual disk resources.
- Attached a Windows ISO image.
- Started the guest installation workflow.

Evidence:

<img width="468" height="164" alt="Oracle VirtualBox download page" src="https://github.com/user-attachments/assets/a86c5e90-e3ff-4b84-ab4d-208a2b13a782" />

<img width="449" height="199" alt="VirtualBox installation wizard" src="https://github.com/user-attachments/assets/f6759513-5b06-47cd-ad96-93be366a7ccb" />

<img width="459" height="246" alt="Creating a Windows 10 virtual machine" src="https://github.com/user-attachments/assets/d0ce9fda-1416-46d9-b353-a7993fc66734" />

<img width="464" height="249" alt="Allocating VM memory" src="https://github.com/user-attachments/assets/e21f71d3-39e6-444e-85c0-c72447b73d0f" />

<img width="430" height="219" alt="Windows ISO attached to VM" src="https://github.com/user-attachments/assets/b707137b-1260-49bf-b0a6-394de96e0068" />

<img width="460" height="374" alt="Windows installation inside VirtualBox" src="https://github.com/user-attachments/assets/a8583d6a-9e92-4a99-9aa6-6fb3a4d307bc" />

## Skills Demonstrated

- Virtualization concepts
- Windows Sandbox setup
- Oracle VirtualBox installation
- Guest operating system provisioning
- ISO-based VM installation
- Security lab isolation
- Host vs. guest environment separation

## Portfolio Summary

This project demonstrates the ability to prepare safe, isolated environments for cybersecurity testing. A clean VM or sandbox is a foundational skill for malware analysis practice, application review, browser testing, and defensive tooling evaluation.
