

- UIKit
- UIPrintInfo
-  duplex 

Instance Property

# duplex

The duplex mode to use for the print job.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var duplex: UIPrintInfo.Duplex { get set }
```

## Discussion

Some printers can print either duplex (double-sided) or single-sided. If double-sided is selected, a printer can either print flipping the back page along the long edge of the paper or along the short edge. The default option for duplex-capable printers is based on document type: single-sided (none) for photos, double-sided and long edge for other documents. If a printer is capable of duplex printing, a switch in the printing options allows users to toggle between single-side and double-sided printing. See the description of the UIPrintInfo.Duplex constants for more information.

## See Also

### Managing print-job attributes

enum Duplex

Constants that describe the duplex mode of a selected printer.

var jobName: String

The name of the print job.

var orientation: UIPrintInfo.Orientation

The orientation of the printed content, portrait or landscape.

enum Orientation

Constants that describe the orientation of printing on a page.

var outputType: UIPrintInfo.OutputType

The kind of printable content.

enum OutputType

Constants that describe the output type, which is an indication of the type of content the app is drawing or providing.

var printerID: String?

An identifier of the printer to use for the print job.

