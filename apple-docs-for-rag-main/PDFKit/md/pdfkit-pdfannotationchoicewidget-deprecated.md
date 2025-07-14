

- PDFKit
-  PDFAnnotationChoiceWidget Deprecated

Class

# PDFAnnotationChoiceWidget

A `PDFAnnotationChoiceWidget` object provides user interactivity on a page of a PDF document, in the form of pop-up menus and lists.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationChoiceWidget
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

`PDFAnnotationChoiceWidget` inherits general annotation behavior from the `PDFAnnotation` class. If you use a `PDFAnnotationChoiceWidget` object, your application must handle hit testing, unless you are simply using `PDFView` to display content. This is because `PDFView` automatically handles hit testing for you.

## Topics

### Getting and Setting the String Value

func stringValue() -> String!

Returns the selection in the widget annotation.

func setStringValue(String!)

Sets the selection in the widget annotation.

### Managing Font and Background Color Characteristics

func backgroundColor() -> NSColor!

Returns the color of the widget annotation background.

func setBackgroundColor(NSColor!)

Sets the background color of the widget annotation.

func font() -> NSFont!

Returns the font used to display the text in the widget annotation.

func setFont(NSFont!)

Sets the font used to display the text in the widget annotation.

func fontColor() -> NSColor!

Returns the font color used to display the text in the widget annotation.

func setFontColor(NSColor!)

Sets the font color used to display the text in the widget annotation.

### Managing the Associated Field Name

func fieldName() -> String!

Returns the internal field name associated with the widget annotation.

func setFieldName(String!)

Sets the internal field name associated with the widget annotation’s value.

### Determining the Type of Choice Widget Annotation

func isListChoice() -> Bool

Returns a Boolean value indicating whether the widget annotation is a list.

func setIsListChoice(Bool)

Sets whether the widget annotation is a list.

### Accessing the Items in the Choice Widget Annotation

func choices() -> [Any]!

Returns an array of strings that represent the items available in the list or pop-up menu of the choice widget annotation.

func setChoices([Any]!)

Sets the items available in the list or pop-up menu of the choice widget annotation.

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

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

