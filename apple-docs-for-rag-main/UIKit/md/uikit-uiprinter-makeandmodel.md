

- UIKit
- UIPrinter
-  makeAndModel 

Instance Property

# makeAndModel

A string that contains the manufacturer’s name and the model name of the printer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var makeAndModel: String? { get }
```

## Discussion

The string in this property is provided by the printer and usually consists of the manufacturer’s name, the model name of the printer, and the model number of the printer.

For printers you create yourself using the init(url:) method, the value of this property is `nil` until you successfully connect to the printer using the contactPrinter(_:) method.

## See Also

### Getting the printer information

var displayName: String

The human-readable printer name.

var displayLocation: String?

The human-readable text that describes the location of the printer.

var supportedJobTypes: UIPrinter.JobTypes

The capabilities of the printer.

struct JobTypes

Constants that indicate the types of jobs that the printer supports.

var supportsColor: Bool

A Boolean value that indicates whether the printer supports color printing.

var supportsDuplex: Bool

A Boolean value that indicates whether the printer supports printing on both sides of a sheet of paper.

