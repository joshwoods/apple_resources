

- UIKit
- UIPrinter
-  displayLocation 

Instance Property

# displayLocation

The human-readable text that describes the location of the printer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var displayLocation: String? { get }
```

## Discussion

Many printers can be configured with a location string to reflect the printer’s physical location in an office. This property contains that location string or `nil` if no such string is available.

For printers you create yourself using the init(url:) method, the value of this property is `nil` until you successfully connect to the printer using the contactPrinter(_:) method.

## See Also

### Getting the printer information

var displayName: String

The human-readable printer name.

var makeAndModel: String?

A string that contains the manufacturer’s name and the model name of the printer.

var supportedJobTypes: UIPrinter.JobTypes

The capabilities of the printer.

struct JobTypes

Constants that indicate the types of jobs that the printer supports.

var supportsColor: Bool

A Boolean value that indicates whether the printer supports color printing.

var supportsDuplex: Bool

A Boolean value that indicates whether the printer supports printing on both sides of a sheet of paper.

