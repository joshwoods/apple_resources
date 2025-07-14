

- UIKit
- UIPrinter
-  supportsColor 

Instance Property

# supportsColor

A Boolean value that indicates whether the printer supports color printing.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var supportsColor: Bool { get }
```

## Discussion

The value of this property is true if the printer supports color printing or false if it does not. For printers you create yourself using the init(url:) method, the value of this property is false until you successfully connect to the printer using the contactPrinter(_:) method.

## See Also

### Getting the printer information

var displayName: String

The human-readable printer name.

var displayLocation: String?

The human-readable text that describes the location of the printer.

var makeAndModel: String?

A string that contains the manufacturer’s name and the model name of the printer.

var supportedJobTypes: UIPrinter.JobTypes

The capabilities of the printer.

struct JobTypes

Constants that indicate the types of jobs that the printer supports.

var supportsDuplex: Bool

A Boolean value that indicates whether the printer supports printing on both sides of a sheet of paper.

