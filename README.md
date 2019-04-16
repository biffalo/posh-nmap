# posh-nmap
Powershell Script to do nmap from powershell, export results to xml, auto pop results in IE/Edge, prompts for customer name and IP

Quick rundown of what this does for transparency:

-installs chocolatey

-installs nmap via chocolately (this puts nmap in path as well)

-invokes nmap with follwing switches -T4 -A -v -Pn (intense scan no ping)

-prompts you for customer name and IP/DNS name you wish to scan

-creates C:\nmap-scans\

-dumps your nmap scan to C:\nmap-scans\$clientname-results.xml

-invokes and pops it in edge/IE assuming that is your file association. Edge/IE reads xml style from nmap path and gives you pretty report
