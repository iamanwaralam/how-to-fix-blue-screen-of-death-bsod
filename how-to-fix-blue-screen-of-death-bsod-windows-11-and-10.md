# How to Fix Blue Screen of Death (BSOD) on Windows 11 and 10

A Blue Screen of Death (BSOD) means Windows hit a critical error it couldn't recover from. Here's a fast, practical way to diagnose and fix it.

## 1. Note the stop code
The blue screen shows a stop code (e.g. IRQL_NOT_LESS_OR_EQUAL, INACCESSIBLE_BOOT_DEVICE). This tells you what actually failed - write it down before you do anything else.

## 2. Check Windows Memory Diagnostic
Press Win+R, type mdsched.exe, and run a restart-and-check. A failing RAM stick is one of the most common BSOD causes.

## 3. Update or roll back your graphics/chipset drivers
A huge share of BSODs trace back to a bad driver update. Check Device Manager for a flagged driver, and update or roll back as needed.

## 4. Run SFC and DISM
Open an elevated Command Prompt and run:
sfc /scannow
DISM /Online /Cleanup-Image /RestoreHealth
These repair corrupted system files that can trigger BSODs.

## 5. Check Event Viewer
Windows Logs > System in Event Viewer will show the exact error that caused the crash, often with the specific driver or file at fault.

## 6. If it keeps happening
A recurring BSOD with the same stop code after the above usually points to failing hardware (RAM, drive, or a loose connection) rather than software.

---
Full step-by-step guide with stop-code-specific fixes: https://techsavvyhelp.com/fix-blue-screen-of-death-bsod/
