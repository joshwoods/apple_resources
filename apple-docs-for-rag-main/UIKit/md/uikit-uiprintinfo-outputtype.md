

- UIKit
- UIPrintInfo
-  outputType 

Instance Property

# outputType

The kind of printable content.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var outputType: UIPrintInfo.OutputType { get set }
```

## Discussion

The output type can be general, photo, or grayscale. An application can set this property to a value thats appropriate to the printable content. The default is UIPrintInfo.OutputType.general. See the descriptions of the UIPrintInfo.OutputType constants for more information.

The output type controls the quality and default paper size used in printing. For example, if your application only prints black text, setting this property to UIPrintInfo.OutputType.grayscale can result in better performance in many cases. See UIPrintPaper for details.

## See Also

### Managing print-job attributes

var duplex: UIPrintInfo.Duplex

The duplex mode to use for the print job.

enum Duplex

Constants that describe the duplex mode of a selected printer.

var jobName: String

The name of the print job.

var orientation: UIPrintInfo.Orientation

The orientation of the printed content, portrait or landscape.

enum Orientation

Constants that describe the orientation of printing on a page.

enum OutputType

Constants that describe the output type, which is an indication of the type of content the app is drawing or providing.

var printerID: String?

An identifier of the printer to use for the print job.

