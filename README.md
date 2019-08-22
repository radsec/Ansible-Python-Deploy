## Ansible-Python-Deploy-Role
Configures ePO agent components on Amazon Linux 2, Red Hat Enterprise Linux, CentOS, and Windows Server 2012 R2+ operating systems.


## System Requirements
```
Ansible 2.5+
Amazon Linux 2, Red Hat Enterprise Linux, CentOS, or Windows Server 2012 R2+
```
## Roles
```
role: epo_agent_deploy
```
## Variables
```
windows_dest: "C:\\ProgramData\\test\epo_agent.exe" #PATH_TO_PLACE_AND_NAME_INSTALLER-PROPERLY ESCAPE SLASHES
windows_url: "https://epo.internal.corp.com/windowsURL"
windows_product_id: "{39290-23949-23949234-92394}" #Retrieve the product id from registry. You can find product ids for installed programs in the Windows registry editor either at HKLM:Software\Microsoft\Windows\CurrentVersion\Uninstall or for 32 bit programs at HKLM:Software\Wow6432Node\Microsoft\Windows\CurrentVersion\Uninstall.
linux_dest: "\tmp\epo_agent.sh"
linux_url: "https://epo.internal.corp.com/linuxURL"
validate_certs: yes #Check for validated certificates "yes" or "no"

```
## License
This Source Code Form is subject to the terms of the Mozilla Public
License, v. 2.0. If a copy of the MPL was not distributed with this
file, You can obtain one at https://mozilla.org/MPL/2.0/.
