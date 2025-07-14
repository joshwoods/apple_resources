

- PDFKit
-  PDFDestination 

Class

# PDFDestination

A `PDFDestination` object describes a point on a PDF page.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFDestination
```

## Overview

In typical usage, you do not initialize `PDFDestination` objects but rather get them as either attributes of PDFAnnotationLink or PDFOutline objects, or in response to the `PDFView` method currentDestination.

## Topics

### Initializing a Destination

init(page: PDFPage, at: CGPoint)

Initializes the destination.

### Getting Pages and Points

var page: PDFPage?

Returns the page that the destination refers to.

var point: CGPoint

Returns the point, in page space, that the destination refers to.

let kPDFDestinationUnspecifiedValue: CGFloat

### Getting a Relative Location

func compare(PDFDestination) -> ComparisonResult

Returns a comparison result that indicates the location of the destination in the document, relative to the current position.

### Instance Properties

var zoom: CGFloat

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

### Accessing Information About an Annotation

var page: PDFPage?

Returns the page that the annotation is associated with.

var modificationDate: Date?

Returns the modification date of the annotation.

var userName: String?

Returns the name of the user who created the annotation.

var type: String?

Returns the type of the annotation.

var action: PDFAction?

An object that represents an action for a PDF element, such as a link annotation.

class PDFAction

An action that is performed when, for example, a PDF annotation is activated or an outline item is clicked.

