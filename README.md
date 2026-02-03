# Apexs-AIO – .NET + VC++ All-in-One Installer

**What this AIO is**  
One script to silently install every major **.NET** runtime (1.0 → 10.x) and **Visual C++ Redistributable** (2005 → 2026) — x86 + x64.  

# How to Run

### Do **not** rename or move the subfolders — the script looks for them by **exact name**.

### Method 1 – Easiest (if available)

1. Extract the ZIP file ("AIO-.Net---VC----main.zip")
2. Right-click **Install-AllRuntimes-(RunAdmin!).ps1**
3. Choose **Run with PowerShell as administrator**  
   *(or **Run as administrator** if that's the only option you see)*
4. Let it run — the PowerShell window will show progress
5. When finished you'll see a confirmation message  
   → A log file (`Install-Log-*.txt`) is created in the same folder — check it if anything looks wrong

### Method 2 – When right-click "Run as admin" is missing or doesn't work

1. Extract the ZIP file
2. Open the **Apexs-AIO** folder in File Explorer
3. In the **address bar at the top**, click once → type `cmd` → press Enter  
   → this opens a **Command Prompt** already in the correct folder
4. In the black Command Prompt window, **copy & paste** this single line and press Enter:

   ```cmd
   powershell -ExecutionPolicy Bypass -Command "Start-Process powershell -Verb RunAs -ArgumentList '-NoProfile -File \"Install-AllRuntimes-(RunAdmin!).ps1\"'"
