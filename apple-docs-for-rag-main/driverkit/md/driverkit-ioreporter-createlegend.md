

- DriverKit
- IOReporter
-  createLegend 

Instance Method

# createLegend

Create a legend entry represending this reporter’s channels.

DriverKitiOSiPadOSmacOS

``` source
OSDictionary * createLegend();
```

## Return Value

An IOReportLegendEntry object or `NULL` on failure.

## Discussion

All channels added to the reporter will be represented in the resulting legend entry.

Legends must be published together as an array under the `kIOReportLegendKey` in the I/O Kit registry. The IOReportLegend class can be used to properly combine legend entries from multiple reporters as well as to put channels into groups of interest to observers. When published, individual legend entries share characteristics such as group and sub-group. Multiple IOReporter instances are required to produce independent legend entries which can then be published with different characteristics.

Drivers wishing to publish legends should do so as part of their `::start()` routine. As superclasses *may* have installed legend entries, any existing existing legend should be retrieved and IOReportLegend used to merge it with the new entries.

Recommendations for best practices are forthcoming.

Instead of calling createLegend on your reporter object and then appending it manually to IOReportLegend, one may prefer to call addReporterLegend which creates and appends a reporter’s IOReportLegendEntry in a single call.

Locking: same-instance concurrency SAFE, MAY BLOCK

## See Also

### Instance Methods

addChannel

Add an additional, similar channel to the reporter.

configureReport

Track IOService::configureReport(), provide sizing info

free

updateReport

Produce standard reply to IOService::updateReport()

