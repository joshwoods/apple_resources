

- UIKit
- UIPrintInfo
-  jobName 

Instance Property

# jobName

The name of the print job.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var jobName: String { get set }
```

## Discussion

The name of the print job appears in the Print Center when the job is printing. An app should set this property to a name appropriate to the content that’s printing. The default job name is the app name.

## See Also

### Managing print-job attributes

var duplex: UIPrintInfo.Duplex

The duplex mode to use for the print job.

enum Duplex

Constants that describe the duplex mode of a selected printer.

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

