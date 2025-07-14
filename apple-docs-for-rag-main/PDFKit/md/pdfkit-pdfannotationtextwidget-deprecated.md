

- PDFKit
-  PDFAnnotationTextWidget Deprecated

Class

# PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationTextWidget
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

`PDFAnnotationTextWidget` objects support interactive forms in a PDF document. This object is comparable to an editable `NSTextField` in Cocoa or an edit text view in Carbon.

## Topics

### Working with Annotation Strings

func stringValue() -> String!

Returns the string assigned to the annotation.

func setStringValue(String!)

Sets the string for the annotation.

func maximumLength() -> Int

Returns the maximum number of characters allowed in the annotation string.

func setMaximumLength(Int)

Sets the maximum number of characters allowed in the annotation string.

### Managing the Font and Font Color

func font() -> NSFont!

Returns the font used for the annotation’s text field.

func setFont(NSFont!)

Sets the font used in the text field of the annotation.

func fontColor() -> NSColor!

Returns the font color used for the annotation’s text field.

func setFontColor(NSColor!)

Sets the font color used for the annotation’s text field.

### Managing Background Color, Alignment, and Rotation

func backgroundColor() -> NSColor!

Returns the background color of the annotation text field.

func setBackgroundColor(NSColor!)

Sets the background color of the annotation text field.

func alignment() -> NSTextAlignment

Returns the text alignment setting for the annotation.

func setAlignment(NSTextAlignment)

Sets the text alignment for the annotation.

func rotation() -> Int

Returns the rotation angle of the annotation text field in degrees.

func setRotation(Int32)

Sets the rotation angle of the annotation text field in degrees.

### Working with Field Names

func fieldName() -> String!

Returns the internal name for the annotation text field.

func setFieldName(String!)

Sets the internal field name for the annotation text field.

### Instance Methods

func attributedStringValue() -> NSAttributedString!

func isMultiline() -> Bool

func setAttributedStringValue(NSAttributedString!)

func setIsMultiline(Bool)

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

class PDFAnnotationSquare

A rectangle annotation on a page.

Deprecated

class PDFAnnotationStamp

A `PDFAnnotationStamp` object allows you to display a word or phrase, such as “Confidential,” in a PDF page.

Deprecated

class PDFAnnotationText

A `PDFAnnotationText` object displays as an icon (such as a “sticky note”) attached to a specified point in the PDF document.

Deprecated

