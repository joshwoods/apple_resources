

- PDFKit
-  PDFDocument 

Class

# PDFDocument

An object that represents PDF data or a PDF file and defines methods for writing, searching, and selecting PDF data.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFDocument
```

## Mentioned in 

Adding Custom Graphics to a PDF

## Overview

The other utility classes are either instantiated from methods in `PDFDocument`, as are `PDFPage` and `PDFOutline`; or support it, as do `PDFSelection` and `PDFDestination`.

You initialize a `PDFDocument` object with PDF data or with a URL to a PDF file. You can then ask for the page count, add or delete pages, perform a find, or parse selected content into an `NSString` object.

## Topics

### Initializing Documents

init?(url: URL)

Initializes a `PDFDocument` object with the contents at the specified URL (if the URL is invalid, this method returns `NULL`).

init?(data: Data)

Initializes a `PDFDocument` object with the passed-in data.

init()

Initializes a `PDFDocument` object.

### Reading and Writing PDFs

Read Operations

Operations that let you access documents and pages, manage document security, and work with searching and selections.

Write Operations

Operations that let you write document data to different locations.

### Setting the Delegate

var delegate: (any PDFDocumentDelegate)?

The object acting as the delegate for the `PDFDocument` object.

protocol PDFDocumentDelegate

The delegate for the `PDFDocument` object.

### Constants

enum PDFDocumentPermissions

An enumeration that specifies document permissions status.

struct PDFDocumentAttribute

A structure that specifies document attributes.

struct PDFDocumentWriteOption

A structure that specifies file writing options for a document.

### Instance Properties

var accessPermissions: PDFAccessPermissions

### Instance Methods

func selection(from: PDFPage, at: CGPoint, to: PDFPage, at: CGPoint, with: PDFSelectionGranularity) -> PDFSelection?

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Content Model

class PDFPage

`PDFPage`, a subclass of `NSObject`, defines methods used to render PDF pages and work with annotations, text, and selections.

class PDFOutline

A `PDFOutline` object is an element in a tree-structured hierarchy that can represent the structure of a PDF document.

class PDFSelection

A `PDFSelection` object identifies a contiguous or noncontiguous selection of text in a PDF document.

