

- DriverKit
-  IOReporter 

Class

# IOReporter

DriverKitiOSiPadOSmacOS

``` source
class IOReporter;
```

## Topics

### Instance Methods

addChannel

Add an additional, similar channel to the reporter.

configureReport

Track IOService::configureReport(), provide sizing info

createLegend

Create a legend entry represending this reporter’s channels.

free

updateReport

Produce standard reply to IOService::updateReport()

### Type Methods

configureAllReports

Calls `configureReport()` on multiple `IOReporter` objects

updateAllReports

Calls `updateReport()` on multiple IOReporter objects.

## Relationships

### Inherits From

- OSObject

### Inherited By

- IOHistogramReporter
- IOSimpleReporter
- IOStateReporter

## See Also

### Classes

IOHistogramReporter

IOReportLegend

IOServiceStateNotificationDispatchSource

IOSimpleReporter

IOStateReporter

OSBundle

OSMappedFile

