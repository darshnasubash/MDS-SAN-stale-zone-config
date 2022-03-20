# MDS-SAN-stale-zone-config
Python script to detect stale zone and device-alias runtime config for MDS switches. 

1. Script can be run from any of the servers which can access the switches in the fabric.
2. Script (right now) takes only one switch info; which can be mentioned in switch-info file. (format can be found in switch-info.txt shared along with the script file)
3. The switch should have following configured –
(switch)# feature nxapi
(switch)# nxapi http port 8080
4. Server (where script will be run) should have python3 and all required modules.
5. The script can be run as –
bash-3.2$ python3 cfg-parser.py -f switch-info.txt 
