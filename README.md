# Microsoft Defender Real-Time Protection stop

### Project purpose
- This is the easiest and cleanest way of disabling RTP on Home edition of Windows.
- It provides an alternative to the already existing ways of disabling RTP
- For a comprehensive comparison of each alternative, including pros and cons, check [this page](https://github.com/Tom4tot/Disable-Microsoft-Defender-Real-Time-Protection-solutions).

### Usage guide
- **Setup**
1. Make sure to disable tamper protection first. For that, go to: Windows Security → Virus and threat protection → Virus and threat protection settings (otherwise the task won't work: tamper protection blocks apps from changing real-time protection settings, including PowerShell).
2. Manually disable real-time protection from Windows Security (this should be the last time you need to do it).
3. Import the task.
- **Uninstall**  
If you want to use Real-Time Protection again, just disable/delete the imported task in Task Scheduler. Don't forget to turn back on Tamper protection for increased security.

### Features
- Only uses official Windows features and components (i.e. Task Scheduler and PowerShell).
- Survive restart, updates, scans, etc. 
- Very low on resources.
- Extremely low chances of breaking anything since there is no hack involved (permission bypass, regedit modifications, etc.). Alternatives often break Windows Security completely whereas this allows to keep other features on (except tamper protection, as previously mentioned).
- Should still work after major Windows updates, except if Microsoft changes things significantly.

### [Purpose of disabling RTP and Drawbacks](https://github.com/Tom4tot/Disable-Microsoft-Defender-Real-Time-Protection-solutions#reasons-to-not-disable-rtp)

### Additional information about Task Scheduler
- [learn.microsoft.com - Task Scheduler Overview](https://learn.microsoft.com/en-us/previous-versions/windows/it-pro/windows-server-2008-r2-and-2008/cc721871(v=ws.11)) - official documentation
- [Wikipedia - Windows Task Scheduler](https://en.m.wikipedia.org/wiki/Windows_Task_Scheduler#Column_'Last_Result') - error codes and general information
- [Reddit - Windows Scheduled Tasks - Is it best to use SYSTEM account as the user to run the task where possible? What is a good practice around using an account?](https://www.reddit.com/r/sysadmin/comments/mnej84/windows_scheduled_tasks_is_it_best_to_use_system/) - best practice regarding user choice
- [ss64.com - SCHTASKS](https://ss64.com/nt/schtasks.html) - commands and general documentation

### Credits
[Duttyend](https://github.com/duttyend/)  
[Tom4tot](https://github.com/Tom4tot/)
