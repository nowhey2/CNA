# CNA
A collection of Cobalt Strike Network Aggressor scripts

## pkill pid|name pid|name pid|name
I.e., pkill cmd.exe 1172 2253 xdiag.exe

<ul>
<li>Will kill the process IDs 1172 2253 and whatever pids map back to cmd.exe and xdiag.exe</li>
<li>Mixing names and PIDs will work fine</li>
<li>The matching on names is case sensitive and will not match space in names.</li>
<li>If names are included, will cause a ps to be issued (bps), in order to map the name to a PID.</li>
<li>If names are not included, it will not perform a ps.</li>
</ul>
