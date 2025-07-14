

- PDFKit
-  PDFAnnotationSquare Deprecated

Class

# PDFAnnotationSquare

A rectangle annotation on a page.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationSquare
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

The lineWidth and style properties of the annotation’s associated `PDFBorder` object determines the stroke thickness and style. The color property of the `PDFAnnotation` class determines the stroke color.

## Topics

### Accessor methods

func interiorColor() -> NSColor!

Gets the fill color used for drawing the annotation.

func setInteriorColor(NSColor!)

Sets the fill color used for drawing the annotation.

## Relationships

### Inherits From

- PDFAnnotation

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

### Deprecated Annotation Types

class PDFAnnotationButtonWidget

A `PDFAnnotationButtonWidget` object provides user interactivity on a page of a PDF document. There are three types of buttons available: push button, radio button, and checkbox.

Deprecated

class PDFAnnotationChoiceWidget

A `PDFAnnotationChoiceWidget` object provides user interactivity on a page of a PDF document, in the form of pop-up menus and lists.

Deprecated

class PDFAnnotationCircleDeprecated

class PDFAnnotationFreeText

A `PDFAnnotationFreeText` object displays text on a page.

Deprecated

class PDFAnnotationInkDeprecated

class PDFAnnotationLine

A `PDFAnnotationLine` object displays a single line on a page.

Deprecated

class PDFAnnotationLinkDeprecated

class PDFAnnotationMarkup

A `PDFAnnotationMarkup` object appears as highlighting, underlining, or a strikethrough style applied to the text of a document.

Deprecated

class PDFAnnotationPopup

A `PDFAnnotationPopup` object provides user interactivity on a PDF page in the form of a pop-up menu.

Deprecated

class PDFAnnotationStamp

A `PDFAnnotationStamp` object allows you to display a word or phrase, such as “Confidential,” in a PDF page.

Deprecated

class PDFAnnotationText

A `PDFAnnotationText` object displays as an icon (such as a “sticky note”) attached to a specified point in the PDF document.

Deprecated

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

