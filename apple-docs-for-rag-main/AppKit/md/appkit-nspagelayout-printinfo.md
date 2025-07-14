

- AppKit
- NSPageLayout
-  printInfo 

Instance Property

# printInfo

The printing information object used when the page layout panel is run.

macOS

``` source
@MainActor
var printInfo: NSPrintInfo? { get }
```

## Discussion

The NSPrintInfo object is set using the beginSheet(with:modalFor:delegate:didEnd:contextInfo:) or runModal(with:) method. The shared NSPrintInfo object is used if the receiver is run using runModal().

## See Also

### Accessing the printing information

class NSPrintInfo

An object that stores information that’s used to generate printed output.

enum Result

