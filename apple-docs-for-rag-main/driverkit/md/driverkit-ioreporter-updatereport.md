

- DriverKit
- IOReporter
-  updateReport 

Instance Method

# updateReport

Produce standard reply to IOService::updateReport()

DriverKitiOSiPadOSmacOS

``` source
IOReturn updateReport(IOReportChannelList * channelList, IOReportConfigureAction action, uint32_t & elementCount, uint8_t * & buffer, size_t & capacity);
```

## Parameters 

`channelList`  

Channels to update

`action`  

Copy/trace data (see `IOReportTypes.h`)

`elementCount`  

Element count.

`buffer`  

Buffer.

`capacity`  

Capacity.

## Return Value

Appropriate IOReturn code

## Discussion

This method searches channelList for channels tracked by this reporter, writes the corresponding data into ‘destination’, and updates ‘result’. It should be possible to pass a given set of UpdateReport arguments to any and all reporters as well as to `super::updateReport()` and get the right result.

The static \`\`IOReporter/updateAllReports\` will call this method on an OSSet of reporters.

Locking: same-instance concurrency SAFE, WILL NOT BLOCK

## See Also

### Instance Methods

addChannel

Add an additional, similar channel to the reporter.

configureReport

Track IOService::configureReport(), provide sizing info

createLegend

Create a legend entry represending this reporter’s channels.

free

