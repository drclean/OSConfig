To enable OEM Folders create the following directories:

$OEM$		This is the current Directory you are in
$OEM$\$$	Files in this directory will be copied to C:\Windows
$OEM$\$$ x64	Files in this directory will be copied to C:\Windows on x64 Computers.  There is a space in the directory name
$OEM$\$$ x86	Files in this directory will be copied to C:\Windows on x86 Computers.  There is a space in the directory name
$OEM$\$1	Files in this directory will be copied to C:\
$OEM$\$$ x64	Files in this directory will be copied to C:\ on x64 Computers.  There is a space in the directory name
$OEM$\$$ x86	Files in this directory will be copied to C:\ on x86 Computers.  There is a space in the directory name


Example:
CMTrace.exe is Architecture specific.  If you want to add CMTrace.exe to all Windows Deployments complete the following:
Copy x86 version of CMTrace.exe to OSConfig\Windows\$OEM$\$$ x86\System32\CMTrace.exe
Copy x64 version of CMTrace.exe to OSConfig\Windows\$OEM$\$$ x64\System32\CMTrace.exe