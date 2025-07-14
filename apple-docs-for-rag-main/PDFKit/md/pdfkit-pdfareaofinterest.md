

- PDFKit
-  PDFAreaOfInterest 

Structure

# PDFAreaOfInterest

The mouse position over PDF view areas.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
struct PDFAreaOfInterest
```

## Overview

These constants are components of a bit field and may be combined arbitrarily.

## Topics

### Constants

static var pageArea: PDFAreaOfInterest

The mouse is over a page.

static var textArea: PDFAreaOfInterest

The mouse is over text.

static var annotationArea: PDFAreaOfInterest

The mouse is over an annotation.

static var linkArea: PDFAreaOfInterest

The mouse is over a link.

static var controlArea: PDFAreaOfInterest

The mouse is over a control.

static var textFieldArea: PDFAreaOfInterest

The mouse is over a text field.

static var iconArea: PDFAreaOfInterest

The mouse is over an icon.

static var popupArea: PDFAreaOfInterest

The mouse is over a popup menu.

static var imageArea: PDFAreaOfInterest

The mouse is over an image.

### Initializers

init(rawValue: Int)

### Type Properties

static var anyArea: PDFAreaOfInterest

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Working with Mouse Position and Events

func areaOfInterest(forMouse: UIEvent) -> PDFAreaOfInterest

Returns the type of area the mouse cursor is over.

func areaOfInterest(for: CGPoint) -> PDFAreaOfInterest

Returns the type of area for a specific cursor location point.

func setCursorFor(PDFAreaOfInterest)

Sets the type of mouse cursor according to the type of area the mouse cursor is over.

func perform(PDFAction)

Performs the specified action.

Drag Operations

Define drag operations allowed for a view.

