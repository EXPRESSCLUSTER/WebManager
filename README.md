# How to start ECX3.x WebManager on today's OS

ECX3.x WebManager is imprelemted as Java Applet. Oracle and MS had given up to support Java Applet and IE.  
This document describes just the procedure for running ECX WebManager on today's Windows without IE and also Linux.

## Java on Windows 

1. Download Java7 (32bit) from [Oracle](https://www.oracle.com/java/technologies/javase/javase7-archive-downloads.html) and install it on WS2019 with default options.
2. Open [ Configure Java ] in Windows Start menu
	1. Goto [ Security ] tab
	2. Select [ Medium ] for [ Security Level ]
	3. [ OK ]
3. Open Windows command prompt then issue the follows

		cd "\Program Files (x86)\Java\jre7\bin"
		javaws.exe http://localhost:29003/main.jnlp

4. [ Security Warning ] dialogue is opend
5. Make [ I accept the risk and want to run this application. ] checked
6. [ Run ]


## Icedtea on Linux

On Linux, *Icedtea* could be used for starting ECX3.x WebManager.
The following command sample was validated on Ubuntu 20.04

	apt install icedtea-netx
	javaws http://localhost:29003/main.hnlp
