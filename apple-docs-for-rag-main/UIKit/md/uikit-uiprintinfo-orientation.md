

- UIKit
- UIPrintInfo
-  orientation 

Instance Property

# orientation

The orientation of the printed content, portrait or landscape.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var orientation: UIPrintInfo.Orientation { get set }
```

## Discussion

An application can set this property to a value thats appropriate to the printable content or it can put up a user interface that enables users to pick the printing orientation. The default value is UIPrintInfo.Orientation.portrait. See the descriptions of the UIPrintInfo.Orientation constants for more information.

Note

UIKit ignores this property when printable content is assigned to the `printingItem` or `printingItems` properties of the shared UIPrintInteractionController object. It determines the orientation based on the type of content.

## See Also

### Managing print-job attributes

var duplex: UIPrintInfo.Duplex

The duplex mode to use for the print job.

enum Duplex

Constants that describe the duplex mode of a selected printer.

var jobName: String

The name of the print job.

enum Orientation

Constants that describe the orientation of printing on a page.

var outputType: UIPrintInfo.OutputType

The kind of printable content.

enum OutputType

Constants that describe the output type, which is an indication of the type of content the app is drawing or providing.

var printerID: String?

An identifier of the printer to use for the print job.

