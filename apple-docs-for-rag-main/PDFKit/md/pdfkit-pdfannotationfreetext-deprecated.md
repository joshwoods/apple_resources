

- PDFKit
-  PDFAnnotationFreeText Deprecated

Class

# PDFAnnotationFreeText

A `PDFAnnotationFreeText` object displays text on a page.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationFreeText
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

Unlike a `PDFAnnotationText` object, a `PDFAnnotationFreeText` object has no open or closed state; its text is always visible. The text annotation performed in Preview uses `PDFAnnotationFreeText`.

The `PDFAnnotation` class’s contents property lets you get and set the textual content for a `PDFAnnotationFreeText` object.

## Topics

### Managing Text Alignment

func alignment() -> NSTextAlignment

Returns the horizontal alignment of text within the bounds of the annotation.

func setAlignment(NSTextAlignment)

Sets the horizontal alignment of text within the bounds of the annotation.

### Managing Font and Font Color

func font() -> NSFont!

Returns the font used for the annotation’s text field.

func setFont(NSFont!)

Sets the font used in the text field of the annotation.

func fontColor() -> NSColor!

Returns the font color used in the text field of the annotation.

func setFontColor(NSColor!)

Sets the font color used in the text field of the annotation.

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

