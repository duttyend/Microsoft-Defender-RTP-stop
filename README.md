# Microsoft-Defender-RTP-stop

### Usage guide
- Make sure you disable tamper protection first in: Windows Security → Virus and threat protection → Virus and threat protection settings (otherwise the task won't work: tamper protection blocks apps from changing real-time protection settings, including powershell)
- Manually disable real-time protection from Windows Security (this should be the last time you need to do it)
- Import the task and make sure to change the user account: change user or Group... → Advanced → Find Now → 'pick your username' → OK

### Benefits from this approach compared to alternatives
- Only uses official Windows features and components (i.e. Task Scheduler and Powershell)
- Very low on resources
- Extreme low chances of breaking anything since there is no hack involved (permission bypass, regedit modifications, etc.)
- Very easy to uninstall / pause temporarily: just disable or delete the task
- Should still after major Windows updates, except if Microsoft changes things significantly
