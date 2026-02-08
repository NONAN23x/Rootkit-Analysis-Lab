# A case study on Linux Kernel Mode Rootkit
A Rootkit is a type of malicious software designed to provide unauthorised, covert access to a computer system while masking its presence. Rootkits can hide files, processes, or system data, making detection difficult and allowing attackers to maintain persistent control over a compromised system.

This lab features Diamorphine, a Linux Kernel Mode Rootkit for versions: 2.6.x/3.x/4.x/5.x/6.x (x86/x86_64 and ARM64)

> Key Features of Diamorphine:
- When loaded, the module starts invisible
- Hide/unhide any process by sending a kill signal 31
- Sending a kill signal 63(to any pid) makes the module become (in)visible
- Sending a kill signal 64(to any pid) makes the given user become root
- Files or directories starting with the MAGIC_PREFIX become invisible;

## Video Demonstration
[![Rootkit Analysis Lab](https://img.youtube.com/vi/dT7OjV9CKVU/0.jpg)](https://www.youtube.com/watch?v=dT7OjV9CKVU)

## Lab Requirements
Lab requirements will be added later.

## Mitigation
In this experiment, we explored the functionality and impact of the Diamorphine rootkit in a controlled environment. By successfully installing and using the rootkit, we observed its ability to hide processes, files, and activities from standard system monitoring tools. This experiment highlighted how rootkits operate at the kernel level to manipulate system behavior stealthily. Understanding these techniques is crucial for developing effective detection and mitigation strategies, emphasizing the importance of regular system audits, kernel integrity monitoring, and proactive defenses to safeguard against such threats in real-world scenarios

Tools like rkhunter (Rootkit Hunter) and chkrootkit are widely used for detecting and mitigating rootkits. These tools scan for common rootkit signatures, hidden files, and unusual configurations. Implementing these tools as part of routine system security measures can enhance detection capabilities and provide an additional layer of defense against stealthy threats.