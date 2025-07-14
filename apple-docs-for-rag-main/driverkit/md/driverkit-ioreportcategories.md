

- DriverKit
-  IOReportCategories 

Type Alias

# IOReportCategories

DriverKitiOSiPadOSmacOS

``` source
typedef uint16_t IOReportCategories;
```

## Discussion

IOReportCategories is the type for the .categories field of IOReportChanelType. These categories are inteded to empower a limited number of clients to retrieve a broad range of channels without knowing much about them. They can be OR’d together as needed. Groups and subgroups are a more extensible mechanism for aggregating channels produced by different drivers.

## See Also

### Data Types

IOCallOnceBlock

IOCallOnceFlag

IOCommand

IOCommandPool

IOCommandPoolPtr

IOCommandPtr

IODMACommand

An object that converts memory references to I/O bus addresses.

IODMACommandSpecification

IODispatchAction

IOHistogramReporter_IVars

IOReportLegendEntry

IOReporter_IVars

IOSimpleReporter_IVars

IOStateReporter_IVars

IOStateReporter_valueSelector

