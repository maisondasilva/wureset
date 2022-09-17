Run wureset.bat and reboot PC

net stop wuauserv
net stop bits
cd %windir%
ren SoftwareDistribution SoftwareDistribution.old
net stop cryptsvc
cd %windir%\System32
ren Catroot Catroot.old
ren Catroot2 Catroot2.old
