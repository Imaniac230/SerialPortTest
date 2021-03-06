# SerialPortTest

A small program that attempts to check and verify data flow through TxD and RxD pins on an RS232 serial interface.
This project was created as a part of a small school assignment.

## Platform
* Tested in Visual Studio 2017 with default compiler (v141).
* **OS:** Windows 10 Home & Professional, Windows 7
* **CPU:** Intel i5 7600K, Intel i5 8300H, AMD FX-8350
* **Port:** USB to RS232 cable and native serial port on MSI Z270 Sli Plus

##	Problems
* Currently only the infinite loop option is functional.
* Detection of a correct received character is now NOT implemented.
* Trying to re-send another data string or reconnecting to a new com port within the application seems to break the functionality.
* Occasional BSOD when using the FX-8350 CPU.
* Too may kernel calls when sending data.
* The code is a complete mess.

## Sources
Overlapped mode implemented using https://docs.microsoft.com/en-us/previous-versions/ff802693(v=msdn.10)