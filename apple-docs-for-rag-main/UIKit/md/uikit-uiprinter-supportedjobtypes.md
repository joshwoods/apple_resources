

- UIKit
- UIPrinter
-  supportedJobTypes 

Instance Property

# supportedJobTypes

The capabilities of the printer.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var supportedJobTypes: UIPrinter.JobTypes { get }
```

## Discussion

Job types indicate the types of operations you can perform with the printer. You might use this information when deciding whether or not to use a printer for a particular task. For example, a photo app might prevent a printer picker interface from displaying printers that do not support the photo job type.

For printers you create yourself using the init(url:) method, the value of this property is unknown until you successfully connect to the printer using the contactPrinter(_:) method.

## See Also

### Getting the printer information

var displayName: String

The human-readable printer name.

var displayLocation: String?

The human-readable text that describes the location of the printer.

var makeAndModel: String?

A string that contains the manufacturer’s name and the model name of the printer.

struct JobTypes

Constants that indicate the types of jobs that the printer supports.

var supportsColor: Bool

A Boolean value that indicates whether the printer supports color printing.

var supportsDuplex: Bool

A Boolean value that indicates whether the printer supports printing on both sides of a sheet of paper.

