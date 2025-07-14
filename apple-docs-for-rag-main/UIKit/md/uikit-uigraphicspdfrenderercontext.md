

- UIKit
-  UIGraphicsPDFRendererContext 

Class

# UIGraphicsPDFRendererContext

The drawing environment for a PDF renderer.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
class UIGraphicsPDFRendererContext
```

## Overview

When using the UIGraphicsPDFRenderer drawing methods, you must pass a block of type UIGraphicsPDFRenderer.DrawingActions as an argument, which provides a UIGraphicsPDFRendererContext instance as an argument. Use the context object to access high-level drawing functions and the underlying Core Graphics context.

Note

UIGraphicsPDFRendererContext inherits much of its functionality from its abstract superclass UIGraphicsRendererContext.

To learn how to use a UIGraphicsPDFRendererContext object in combination with a PDF renderer, see Creating a graphics PDF renderer.

## Topics

### Marking new pages

func beginPage()

Marks the beginning of a new page in the PDF context and configures it using default values.

func beginPage(withBounds: CGRect, pageInfo: [String : Any])

Marks the beginning of a new page in the PDF context and configures it using the specified values.

### Getting the PDF bounds

var pdfContextBounds: CGRect

The bounds of the PDF context for the current page.

### Managing destinations

func addDestination(withName: String, at: CGPoint)

Creates a named destination point in the current PDF page.

func setDestinationWithName(String, for: CGRect)

Creates a link rectangle in the current page that jumps the PDF viewer to the named destination when clicked.

func setURL(URL, for: CGRect)

Creates a link to an external resource defined by a URL

## Relationships

### Inherits From

- UIGraphicsRendererContext

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Graphics contexts

class UIGraphicsRenderer

An abstract base class for creating graphics renderers.

class UIGraphicsRendererContext

The base class for the drawing environments for graphics renderers.

class UIGraphicsRendererFormat

A set of drawing attributes that represents the configuration of a graphics renderer context.

class UIGraphicsImageRenderer

A graphics renderer for creating Core Graphics-backed images.

class UIGraphicsImageRendererContext

The drawing environment for an image renderer.

class UIGraphicsImageRendererFormat

A set of drawing attributes that represents the configuration of an image renderer context.

class UIGraphicsPDFRenderer

A graphics renderer for creating PDFs.

class UIGraphicsPDFRendererFormat

A set of drawing attributes that represents the configuration of a PDF renderer context.

