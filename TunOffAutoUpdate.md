##############################
//\\ Turn Off Auto Update //\\
||||||||||||||||||||||||||||||

/*********************************************************\
|  Block Windows 10 Automatic Updates Using Group Policy  |
***********************************************************
	Open "gpedit.msc".
	GoTo The Path "Computer Configuration > Administrative Templates > Windows Components > Windows Update".
	Double Click on "Configure Automatic Updates".
	Check the “Disabled” option to turn off the policy.
	Click on the "Apply Button".
	Click on “Ok” button

/*********************************************************\
|    Block Windows 10 Automatic Updates Using Registry    |
***********************************************************
	Open “regedit”.
	Navigate to "HKEY_LOCAL_MACHINE\SOFTWARE\POLICIES\MICROSOFT\WINDOWS".
	Right-click on the “Windows” folder and select “New” and then click on “Key” option.
	Name the new key as “Windows Update” and press on enter.
	Right-click on the new key and select new and click on “Key” button.
	Name the New key “AU” and press on enter
	Rick click on the right side of the screen and Select “new” and select “DWORD (32-Bit) Value.
	Name the New Key as “NoAutoUpdate” and hit Enter.
	Double click on the new key and change the value from “0” to “1”.
	Click on “Ok”.
	Restart your computer to apply changes.