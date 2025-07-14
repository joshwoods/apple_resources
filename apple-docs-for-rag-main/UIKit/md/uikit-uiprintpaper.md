

- UIKit
-  UIPrintPaper 

Class

# UIPrintPaper

The size of paper for a print job and the rectangular area that the content prints within.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UIPrintPaper
```

## Overview

In most cases, UIKit automatically creates an instance of UIPrintPaper that is appropriate for a print job. The UIKit framework has default paper sizes based on a print job’s output type (outputType is a property of the UIPrintInfo class). If the output type is UIPrintInfo.OutputType.photo, the default paper size is 4x6 or A6 or some other standard size, depending on locale; if the output type is UIPrintInfo.OutputType.general or UIPrintInfo.OutputType.grayscale, the default paper size is US Letter (8 1/2 by 11 inches) or A4 or some other standard size, depending on locale.

Applications may have special requirements for paper sizes. For example, a word-processing application may have items of “stationery” in which printable content must be drawn. If your application fits the special case, the delegate of UIPrintInteractionController can implement the printInteractionController(_:choosePaper:) method of the UIPrintInteractionControllerDelegate protocol to return a suitable print paper object. One way to do this is to call the bestPaper(forPageSize:withPapersFrom:) class method of UIPrintPaper, passing in a array of print paper objects representing the paper sizes supported by a printer. The print paper object returned from this method represents the paper size best matched to the size requirement of the application.

The printable rectangle (printableRect) is the imageable area for the printer on a paper of a given size.

If you are using a UIPrintPageRenderer object to draw the content for printing, the rectangle stored in the printableRect property is stored in the page renderer’s property of the same name and the paper size used for a print job is stored as part of the paperRect property.

## Topics

### Getting the paper size and the printing area

var paperSize: CGSize

The size of the sheet to use for printing.

var printableRect: CGRect

The rectangle that represents the portion of the paper that can be imaged upon.

### Obtaining the best paper size for printing

class func bestPaper(forPageSize: CGSize, withPapersFrom: [UIPrintPaper]) -> UIPrintPaper

The print-paper object that UIKit determines to be the best for a print job based on the specified page size and the paper size–imageable area combinations specific to the printer.

### Deprecated

func printRect() -> CGRect

Deprecated.

Deprecated

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Sendable

## See Also

### Job info

class UIPrinter

A printer on the network.

class UIPrintInfo

Information about a print job that the system uses when it prints.

