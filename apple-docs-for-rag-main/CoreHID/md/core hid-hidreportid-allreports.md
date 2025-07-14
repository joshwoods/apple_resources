

- Core HID
- HIDReportID
-  allReports 

Type Property

# allReports

A convenient definition that represents every possible report ID.

macOS 15.0+

``` source
static let allReports: ClosedRange
```

## Discussion

This can be useful when specifying the report IDs to monitor in monitorNotifications(reportIDsToMonitor:elementsToMonitor:).

