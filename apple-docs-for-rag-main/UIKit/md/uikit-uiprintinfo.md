

- UIKit
-  UIPrintInfo 

Class

# UIPrintInfo

Information about a print job that the system uses when it prints.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPrintInfo
```

## Overview

A UIPrintInfo object encapsulates information about a print job, including printer identifier, job name, output type (photo, normal, grayscale), orientation (portrait or landscape), and any selected duplex mode.

Typically, you create a UIPrintInfo object and assign it to the printInfo property of the shared UIPrintInteractionController instance. However, it isn’t necessary to create a UIPrintInfo object for a print job; UIKit assumes certain defaults. In the printing-options user interface, users can select the printer, single-sided or double-sided printing for duplex printers, and (if the app allows it) a range of pages to print.

## Topics

### Creating a print info object

class func printInfo() -> UIPrintInfo

Returns a print-information object initialized with default values.

init(dictionary: [AnyHashable : Any]?)

Returns a print-information object that is initialized with the data in the passed-in dictionary.

var dictionaryRepresentation: [AnyHashable : Any]

A dictionary representation of a print-information object.

init?(coder: NSCoder)

Creates a print info object from data in an unarchiver.

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

var outputType: UIPrintInfo.OutputType

The kind of printable content.

enum OutputType

Constants that describe the output type, which is an indication of the type of content the app is drawing or providing.

var printerID: String?

An identifier of the printer to use for the print job.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Job info

class UIPrinter

A printer on the network.

class UIPrintPaper

The size of paper for a print job and the rectangular area that the content prints within.

