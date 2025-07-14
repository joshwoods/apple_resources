

- PDFKit
-  PDFAnnotationLine Deprecated

Class

# PDFAnnotationLine

A `PDFAnnotationLine` object displays a single line on a page.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationLine
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

The lineWidth and style properties of the annotation’s associated `PDFBorder` object determines the stroke thickness and style. The color property of the `PDFAnnotation` class determines the stroke color.

## Topics

### Specifying the Starting and Ending Points

func startPoint() -> NSPoint

Returns the starting point for the line.

func setStart(NSPoint)

Sets the starting point for the line.

func endPoint() -> NSPoint

Returns the ending point for the line in page space.

func setEnd(NSPoint)

Sets the ending point for the line.

### Specifying the Line Ending Styles

func startLineStyle() -> PDFLineStyle

Returns the line ending style for the starting point of the line.

func setStart(PDFLineStyle)

Sets the line ending style for the starting point of the line.

func endLineStyle() -> PDFLineStyle

Returns the line ending style for the ending point of the line.

func setEnd(PDFLineStyle)

Sets the line ending style for the ending point of the line.

### Specifying the Color of Line-end Ornaments

func interiorColor() -> NSColor!

Returns the color used to fill the ornament at the ends of the line.

func setInteriorColor(NSColor!)

Sets the color used to fill the ornament at the ends of the line.

### Constants

enum PDFLineStyle

The following constants specify the available line ending styles.

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

class PDFAnnotationLinkDeprecated

class PDFAnnotationMarkup

A `PDFAnnotationMarkup` object appears as highlighting, underlining, or a strikethrough style applied to the text of a document.

Deprecated

class PDFAnnotationPopup

A `PDFAnnotationPopup` object provides user interactivity on a PDF page in the form of a pop-up menu.

Deprecated

class PDFAnnotationSquare

A rectangle annotation on a page.

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

