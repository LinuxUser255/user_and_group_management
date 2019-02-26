#!/bin/bash

#Custom nmap command condensed into concise BASH script.
#This scan initiates service enumeration, syn scan, timing, and OS detection.  

echo "Enter the target IP : " 

read TargetIP 

nmap -p1-65535 -sV -T4 -A $TargetIP -oG BestnmapScan

cat BestnmapScan

./bnmap.sh
