# Persisrence Survivability Rating

## Parameter Syntax: 


### Build Out Path
Current value based supported remote queries:

| Query         | Weighted Value| implemented|
| ------------- |:-------------:|:-----:|
| WmiBootTime        | 40% | Yes   |
| WmiInstallDate     | 5%      | Yes   |
| WmiOS              | 5%      | Yes   |
| WmiServer          | 10%      | Yes   |
| WmiRamSize         | 5%      | Yes   |
| WmiArch            | 5%      | Yes   |
| WmiDisk            | 5%      | Yes   |
| WmiLProcessorCount | 5%      | Yes   |
| WmiProcessorCores  | 5%      | Yes   |
| WmiProcessorSpeed  | 5%      | Yes   |
| WmiProcessCount    | 5%      | Yes   |
| WmiSystemEnclosure | 10%      | Yes   |
| WmiLoggedOnUsers   | centered      | No    |
| WmiCollectorService| centered      | No    |
| WmiNICData         | centered      | No    |
| WmiAVQuery         | centered      | No    |
| WmiPowerSettings   | centered      | No    |
| WmiOSuite          | centered      | No    |
| WmiPointerDevice   | centered      | No    |

Current boolean based supported remote queries:

| Query         | Impact        | implemented|
| ------------- |:-------------:|:-----:|
| WmiPortableOS   | Implant location| Yes    |
| WmiVMChecks     | Truth of data   | Yes    |
| WmiLogging      |Alerts in logging| No    |

### Sample output:
```

PS C:\Users\Administrator\Desktop>  Invoke-FindPersitence 
[*] Top Server locations based on Persistence Survivability rating: 
[*] Top Desktop locations based on Persistence Survivability rating: 
[*] Top VM locations based on Persistence Survivability rating: 


NetBIOSName              : ALEX32-PC.tester.org
IpAddress                : 172.16.168.136
LastBoot                 : 20160509061014.500000-420
InstallDate              : 20150707115729.000000-420
OSArch                   : 64-bit
ServerType               : 1
SystemEnclosure          : 1
RamSize                  : 2
DiskSize                 : 38.6479606628418
ProcessorSpeed           : 2999
ProcessorLogicalCores    : 1
ProcessorCores           : 1
ProcessCount             : 38
PortableOS               : 
VMware                   : True
LastBootV                : 0.3
InstallDateV             : 0.4
OSArchV                  : 0.3
ServerTypeV              : 0.33
SystemEnclosureV         : 0.1
DiskSizeV                : 0.3
RamSizeV                 : 0.5
ProcessorSpeedV          : 1
ProcessorLogicalCoreV    : 0.3
ProcessCountV            : 1
LastBootWV               : 0.12
InstallDateWV            : 0.02
OSArchWV                 : 0.015
ServerTypeWV             : 0.033
SystemEnclosureWV        : 0.01
DiskSizeWV               : 0.015
RamSizeWV                : 0.1
ProcessorSpeedWV         : 0.05
ProcessorLogicalCoreWV   : 0.015
ProcessCountWV           : 0.05
PersistenceSurvivability : 0.378

NetBIOSName              : ALEX2-PC.tester.org
IpAddress                : 172.16.168.160
LastBoot                 : 20160508162848.500000-420
InstallDate              : 20150707115729.000000-420
OSArch                   : 64-bit
ServerType               : 1
SystemEnclosure          : 1
RamSize                  : 2
DiskSize                 : 48.5253257751465
ProcessorSpeed           : 2999
ProcessorLogicalCores    : 1
ProcessorCores           : 1
ProcessCount             : 32
PortableOS               : 
VMware                   : True
LastBootV                : 0.3
InstallDateV             : 0.4
OSArchV                  : 0.3
ServerTypeV              : 0.33
SystemEnclosureV         : 0.1
DiskSizeV                : 0.3
RamSizeV                 : 0.5
ProcessorSpeedV          : 1
ProcessorLogicalCoreV    : 0.3
ProcessCountV            : 1
LastBootWV               : 0.12
InstallDateWV            : 0.02
OSArchWV                 : 0.015
ServerTypeWV             : 0.033
SystemEnclosureWV        : 0.01
DiskSizeWV               : 0.015
RamSizeWV                : 0.1
ProcessorSpeedWV         : 0.05
ProcessorLogicalCoreWV   : 0.015
ProcessCountWV           : 0.05
PersistenceSurvivability : 0.378

NetBIOSName              : WIN-2PNK85BO0TD.tester.org
IpAddress                : {fe80::9a7:551a:2614:ae6c%12, 172.16.168.223}
LastBoot                 : 20160227200724.489034-480
InstallDate              : 20150707115648.000000-420
OSArch                   : 64-bit
ServerType               : 2
SystemEnclosure          : 1
RamSize                  : 2
DiskSize                 : 43.868766784668
ProcessorSpeed           : 2999
ProcessorLogicalCores    : 1
ProcessorCores           : 1
ProcessCount             : 73
PortableOS               : False
VMware                   : True
LastBootV                : 0.85
InstallDateV             : 0.4
OSArchV                  : 0.3
ServerTypeV              : 0.66
SystemEnclosureV         : 0.1
DiskSizeV                : 0.3
RamSizeV                 : 0.5
ProcessorSpeedV          : 1
ProcessorLogicalCoreV    : 0.3
ProcessCountV            : 1
LastBootWV               : 0.34
InstallDateWV            : 0.02
OSArchWV                 : 0.015
ServerTypeWV             : 0.066
SystemEnclosureWV        : 0.01
DiskSizeWV               : 0.015
RamSizeWV                : 0.1
ProcessorSpeedWV         : 0.05
ProcessorLogicalCoreWV   : 0.015
ProcessCountWV           : 0.05
PersistenceSurvivability : 0.631

[*] Overall Persistence Survivability stats: 
    Total number of hosts:  3
    Total VMware hosts:  3
    Total Desktop hosts:  0
    Total Server hosts:  0
    Survivability mean:  46 %
```
