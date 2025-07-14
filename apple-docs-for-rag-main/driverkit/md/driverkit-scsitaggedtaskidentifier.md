

- DriverKit
-  SCSITaggedTaskIdentifier 

Type Alias

# SCSITaggedTaskIdentifier

64-bit number to represent a unique task identifier.

DriverKitiOSiPadOSmacOS

``` source
typedef UInt64 SCSITaggedTaskIdentifier;
```

## Discussion

The Tagged Task Identifier is used when a Task has a Task Attribute other than SIMPLE. The SCSI Application Layer client that controls the Logical Unit for which a Task is intended is required to guarantee that the Task Tag Identifier is unique. Zero cannot be used a a Tag value as this is used to when a Tagged Task Identifier value is needed for a Task with a SIMPLE attribute.

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

