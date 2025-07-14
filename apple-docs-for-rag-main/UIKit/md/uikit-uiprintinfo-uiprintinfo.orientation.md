

- UIKit
- UIPrintInfo
-  UIPrintInfo.Orientation 

Enumeration

# UIPrintInfo.Orientation

Constants that describe the orientation of printing on a page.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Orientation
```

## Overview

You use these constants when setting the value of the orientation property of a `UIPrintInfo` object.

Note

UIKit ignores the orientation property when printable content is assigned to the `printingItem` or `printingItems` properties of the shared UIPrintInteractionController object. It determines the orientation based on the type of content.

## Topics

### Constants

case portrait

Pages are printed in portrait orientation.

case landscape

Pages are printed in landscape orientation.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

var outputType: UIPrintInfo.OutputType

The kind of printable content.

enum OutputType

Constants that describe the output type, which is an indication of the type of content the app is drawing or providing.

var printerID: String?

An identifier of the printer to use for the print job.

