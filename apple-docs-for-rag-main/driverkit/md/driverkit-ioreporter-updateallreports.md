

- DriverKit
- IOReporter
-  updateAllReports 

Static Method

# updateAllReports

Calls `updateReport()` on multiple IOReporter objects.

DriverKitiOSiPadOSmacOS

``` source
static IOReturn updateAllReports(OSCollection * reporters, OSData * channels, IOReportConfigureAction action, uint32_t * outElementCount, uint64_t offset, uint64_t capacity, IOMemoryDescriptor * buffer);
```

## Parameters 

`reporters`  

An OSSet of IOReporter objects.

`channels`  

An OSData object containing the list of channels to update.

`action`  

The action to perform.

`outElementCount`  

The number of elements in the response.

`offset`  

The offset in the buffer.

`capacity`  

The capacity of the buffer.

`buffer`  

The buffer to write the response to.

## Return Value

`kIOReturnSuccess` if all objects successfully complete updateReport.

## Discussion

The OSSet must only contain IOReporter instances. The presence of non-`IOReporter` instances will cause this function to return kIOReturnBadArgument. If any reporter returns an error, the function will immediately return that error.

Per the configureReport documentation, each reporter will search channelList for channels it is reporting and provide a partial response.

## See Also

### Type Methods

configureAllReports

Calls `configureReport()` on multiple `IOReporter` objects

