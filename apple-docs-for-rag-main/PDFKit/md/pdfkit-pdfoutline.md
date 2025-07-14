

- PDFKit
-  PDFOutline 

Class

# PDFOutline

A `PDFOutline` object is an element in a tree-structured hierarchy that can represent the structure of a PDF document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFOutline
```

## Overview

An outline is an optional component of a PDF document, useful for viewing the structure of the document and for navigating within it.

Outlines are created by the document’s author. If you represent a PDF document outline using outline objects, the root of the hierarchy is obtained from the PDF document itself. This root outline is not visible and serves merely as a container for the visible outlines.

## Topics

### Initializing an Outline

init()

Initializes a `PDFOutline` object.

### Getting Information About an Outline

var document: PDFDocument?

Returns the document with which the outline is associated.

var numberOfChildren: Int

Returns the number of child outline objects in the outline.

var parent: PDFOutline?

Returns the parent outline object of the outline (returns `NULL` if called on the root outline object).

func child(at: Int) -> PDFOutline?

Returns the child outline object at the specified index.

var index: Int

Returns the index of the outline.

### Managing Outline Labels

var label: String?

Returns the label for the outline.

### Managing Actions and Destinations

var destination: PDFDestination?

Returns the destination associated with the outline.

var action: PDFAction?

Returns the action performed when users click the outline.

### Changing an Outline Hierarchy

func insertChild(PDFOutline, at: Int)

Inserts the specified outline object at the specified index.

func removeFromParent()

Removes the outline object from its parent (does nothing if outline object is the root outline object).

### Managing the Disclosure of an Outline Object

var isOpen: Bool

Returns a Boolean value that indicates whether the outline object is initially disclosed.

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

## See Also

### Content Model

class PDFDocument

An object that represents PDF data or a PDF file and defines methods for writing, searching, and selecting PDF data.

class PDFPage

`PDFPage`, a subclass of `NSObject`, defines methods used to render PDF pages and work with annotations, text, and selections.

class PDFSelection

A `PDFSelection` object identifies a contiguous or noncontiguous selection of text in a PDF document.

