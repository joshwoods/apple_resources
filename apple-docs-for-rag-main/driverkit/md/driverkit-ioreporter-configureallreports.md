

- DriverKit
- IOReporter
-  configureAllReports 

Static Method

# configureAllReports

Calls `configureReport()` on multiple `IOReporter` objects

DriverKitiOSiPadOSmacOS

``` source
static IOReturn configureAllReports(OSCollection * reporters, OSData * channels, IOReportConfigureAction action, uint32_t * outCount);
```

## Parameters 

`reporters`  

An `OSSet` of `IOReporter` objects.

`channels`  

The full list of channels to configure.

`action`  

The action to perform.

`outCount`  

Count of updated reporters.

## Return Value

`kIOReturnSuccess` if all objects successfully complete configureReport.

## Discussion

The OSSet must only contain `IOReporter` instances. The presence of non-`IOReporter` instances will cause this function to return `kIOReturnBadArgument`. If any reporter returns an error, the function will immediately return that error.

Per the configureReport documentation, each reporter will search channelList for channels it is reporting and provide a partial response.

## See Also

### Type Methods

updateAllReports

Calls `updateReport()` on multiple IOReporter objects.

