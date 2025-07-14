

- Core HID
- HIDElement
-  reportID 

Instance Property

# reportID

The report ID for the report that contains this element.

macOS 15.0+

``` source
var reportID: HIDReportID?
```

## Discussion

This may not be populated if the descriptor contains only one report.

