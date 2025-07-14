

- HIDDriverKit
- IOUserHIDEventService
-  processReport 

Instance Method

# processReport

DriverKit 21.0+macOS

``` source
kern_return_t processReport(uint64_t timestamp, uint64_t report, uint32_t reportLength, IOHIDReportType type, uint32_t reportID);
```

