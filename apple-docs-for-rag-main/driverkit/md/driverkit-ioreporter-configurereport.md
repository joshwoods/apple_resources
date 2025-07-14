

- DriverKit
- IOReporter
-  configureReport 

Instance Method

# configureReport

Track IOService::configureReport(), provide sizing info

DriverKitiOSiPadOSmacOS

``` source
IOReturn configureReport(IOReportChannelList * channelList, IOReportConfigureAction action, uint32_t & elementCount);
```

## Parameters 

`channelList`  

Channels to configure.

`action`  

Enable/disable/size, etc (see `IOReportTypes.h`).

`elementCount`  

Element count.

## Return Value

Appropriate `IOReturn` code.

## Discussion

Any time a reporting driver’s ::configureReport method is invoked, this method should be invoked on each IOReporter that is being used by that driver to report channels in channelList.

Any channels in channelList which are not tracked by this reporter are ignored. ::configureReport(kIOReportGetDimensions) expects the full size of all channels, including any reported by superclasses. It is valid to call this routine on multiple reporter objects in succession and they will increment ‘result’ to provide the correct total.

The static IOReporter::configureAllReports() will call this method on multiple reporters grouped in an OSSet.

Locking: same-instance concurrency SAFE, MAY BLOCK

## See Also

### Instance Methods

addChannel

Add an additional, similar channel to the reporter.

createLegend

Create a legend entry represending this reporter’s channels.

free

updateReport

Produce standard reply to IOService::updateReport()

