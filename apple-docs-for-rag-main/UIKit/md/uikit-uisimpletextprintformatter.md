

- UIKit
-  UISimpleTextPrintFormatter 

Class

# UISimpleTextPrintFormatter

An object that lays out plain text for printing, possibly over multiple pages.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
class UISimpleTextPrintFormatter
```

## Overview

The UISimpleTextPrintFormatter class allows you to specify global font, color, and text alignment properties for the printed text. To use this print formatter for a print job, create an instance of UISimpleTextPrintFormatter initialized with the text, set the text properties and the inherited layout properties, and add the object to the print job in one of two ways:

- If a single print formatter is being used for the print job (with no additional drawing), assign it to the printFormatter property of the UIPrintInteractionController shared instance. The inherited startPage property identifies the beginning page of content with which the formatter is associated.

- If you are using multiple formatters along with a page renderer, associate each print formatter with a starting page of the printed content. You often take this approach when you want to add content such as headers and footers to what the formatters provide. You have two ways of associating a print formatter with a UIPrintPageRenderer object:

- You can add print formatters to the printFormatters property of the UIPrintPageRenderer object; the startPage property of the print formatter specifies the starting page.

- You can add print formatters by calling addPrintFormatter(_:startingAtPageAt:) for each print formatter; the second parameter of this method specifies the starting page (and overrides any startPage value).

You can change the text at any time before drawing of the printable content begins. You cannot change the text after drawing begins.

## Topics

### Creating a simple-text print formatter

init(attributedText: NSAttributedString)

Returns a simple-text print formatter initialized with attributed text.

init(text: String)

Returns a simple-text print formatter initialized with plain text.

### Getting and setting the text

var attributedText: NSAttributedString?

A string of attributed text.

var text: String?

A string of plain text.

### Text attributes for printed content

var font: UIFont?

The font of the printed text.

var color: UIColor?

The color of the printed text.

var textAlignment: NSTextAlignment

The alignment of the printed text.

## Relationships

### Inherits From

- UIPrintFormatter

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol
- Sendable

## See Also

### Formatters

class UIPrintFormatter

An abstract base class for print formatters, which are objects that lay out custom printable content that can cross page boundaries.

class UIViewPrintFormatter

An object that lays out the drawn content of a view for printing.

class UIMarkupTextPrintFormatter

An object that lays out HTML text for a multipage print job.

