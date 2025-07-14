

- DriverKit
- IOReporter
-  addChannel 

Instance Method

# addChannel

Add an additional, similar channel to the reporter.

DriverKitiOSiPadOSmacOS

``` source
IOReturn addChannel(uint64_t channelID, const char * channelName);
```

## Parameters 

`channelID`  

Identifier for the channel to be added.

`channelName`  

An optional human-readble name for the channel.

## Return Value

Appropriate `IOReturn` code.

## Discussion

The reporter will allocate memory to track a new channel with the provided ID and name (if any). Its other traits (type, etc) will be those provided when the reporter was initialized. If no channel name is provided and the channelID consists solely of ASCII bytes, those bytes (ignoring any NUL bytes) will be used as the human-readable channel name in user space. The `IOREPORT_MAKEID()` macro in `IOReportTypes.h` can be used to create ASCII channel IDs.

Locking: same-instance concurrency SAFE, MAY BLOCK

## See Also

### Instance Methods

configureReport

Track IOService::configureReport(), provide sizing info

createLegend

Create a legend entry represending this reporter’s channels.

free

updateReport

Produce standard reply to IOService::updateReport()

