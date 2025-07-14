

- AppKit
-  NSPDFInfo 

Class

# NSPDFInfo

An object that stores information associated with the creation of a PDF file, such as its URL, tag names, page orientation, and paper size.

macOS 10.9+

``` source
class NSPDFInfo
```

## Overview

Typically, a PDF panel—that is, a panel created by an NSPDFPanel object—displays the information supplied by an NSPDFInfo object when the user wants to export content as a PDF file. A PDF panel can also update a PDF info object with information it receives from the user.

## Topics

### Specifying PDF Information

var url: URL?

The URL identifying the location at which the PDF file will be created.

var isFileExtensionHidden: Bool

A Boolean value that indicates whether the file extension should appear after the filename.

var tagNames: [String]

An array of tag names that should be applied to the PDF file after it’s created.

var orientation: NSPrintInfo.PaperOrientation

The paper orientation to use when exporting content as a PDF file.

var paperSize: NSSize

The paper size to use when exporting content as a PDF file.

var attributes: NSMutableDictionary

A dictionary of additional attributes that describe how to export content as a PDF file.

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

## See Also

### Vector Formats

class NSPDFImageRep

An object that can render an image from a PDF format data stream.

class NSEPSImageRep

An object that can render an image from encapsulated PostScript (EPS) code.

Deprecated

