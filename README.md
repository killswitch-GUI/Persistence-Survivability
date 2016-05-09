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
