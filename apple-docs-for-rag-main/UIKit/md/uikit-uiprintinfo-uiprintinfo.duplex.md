

- UIKit
- UIPrintInfo
-  UIPrintInfo.Duplex 

Enumeration

# UIPrintInfo.Duplex

Constants that describe the duplex mode of a selected printer.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
enum Duplex
```

## Overview

You use these constants when setting the value of the duplex property of a `UIPrintInfo` object.

## Topics

### Constants

case none

No double-sided (duplex) printing; single-sided printing only.

case longEdge

Duplex printing that flips the back page along the long edge of the paper.

case shortEdge

Duplex print that flips the back page along the short edge of the paper.

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

