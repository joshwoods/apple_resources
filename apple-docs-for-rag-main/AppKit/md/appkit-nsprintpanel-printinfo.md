

- AppKit
- NSPrintPanel
-  printInfo 

Instance Property

# printInfo

The information associated with the running Print panel.

macOS 10.5+

``` source
@MainActor
var printInfo: NSPrintInfo { get }
```

## Discussion

The value in this property is `nil` if the Print panel is not currently running.

## See Also

### Accessing the Printing Information

class NSPrintInfo

An object that stores information that’s used to generate printed output.

enum Result

