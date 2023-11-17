# PcapPoisoning

## Problem
How about some hide and seek heh?
Download this file and find the flag.

## Solution

1. Download the file.
2. Open Windows Subsystem for Linux.
3. Try running the following code.
```
cat trace.pcap 
```
4. On running the abovee command, it gives out a binary output. 
5. To find the flag we can pipe it to string and then grep it, by using the following code.

```
cat trace.pcap |strings -a |grep "pico"
```

## Flag
`picoCTF{P64P_4N4L7S1S_SU55355FUL_f621fa37}`