**Synopsis**
aircrack-ng[options]<inputfile(s)>

**Description**
it can recover the wep key once enough encryped packets have been captured with airodump-ng. This part of the aircrack-ng methods.
The first method is via PTW approach (Pyshkin, Tews, Weinman).
The main advantage of the PTW approach is that very few data packets are required to crack the wep key.
The second method is the FMS/KoreK method.
The FMS/KoreK method incorporates various statistical attacks to discover the wep key and uses these in combination with brute forcing

Additionally, the program offers a dictionary method for determining the wep key.
For cracking WPA/WPA2 pre-shared key, a wordlist (file or stdin) or an airolib-ng has to be used

**Input files**
Capture files(.cap, .pcap), IVS(.ivs) or Hashcat HCCAPX file (.hccapx)

**Options**
Common options: -a <amode>
Force the attack mode: 1 or wep for WEP (802.11) and 2 or wpa for WPA/WPA2 PSK (802.11i and 802.11w)

-e <essid>
Select the target network based on the ESSID.
...

-b <bssid> o -bssid
Select the target network based on the access point MAC address

-p <nbcpu>
Set the option to the number of cpus to use (only available on SMP systems) for cracking the key/passphrase.
By default, it uses all available cpus

-q
if set, no status information is displayed

-C <macs> or -combine
Merges all those APs Mac (separated by a comma) into a virtual one

-I <file>
Write the key into a file. Overwrites the file if it already exists.

STATIC WEP CRACKING OPTIONS: -c
Search alpha-nmeric characters only.

-t
Search binary coded decimal characters only

-h
Search the numeric key for Fritz!Box

-d <mask> or -debug
Specify mask of the key. For example: A1:XX:CF

-m <maddr>
...la suite au prochain épisode

* **See also**
airbase-ng
aireplay-ng
airmon-ng
airodump-ng
airodump-ng-oui-update
airserv-ng
besside-ng
easside-ng
tkiptun-ng
wesside-ng
airdecap-ng
airdecloack-ng
airolib-ng
besside-ng-crawler
buddy-ng
ivstools
kstats
makeivs-ng
packetforge-ng
wpaclean
airventriloquist