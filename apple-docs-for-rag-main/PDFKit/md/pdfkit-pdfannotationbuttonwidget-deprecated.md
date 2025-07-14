

- PDFKit
-  PDFAnnotationButtonWidget Deprecated

Class

# PDFAnnotationButtonWidget

A `PDFAnnotationButtonWidget` object provides user interactivity on a page of a PDF document. There are three types of buttons available: push button, radio button, and checkbox.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationButtonWidget
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

`PDFAnnotationButtonWidget` inherits general annotation behavior from the `PDFAnnotation` class. If you use a `PDFAnnotationButtonWidget` object, your application must handle hit testing, unless you are simply using `PDFView` to display content. This is because `PDFView` automatically handles hit testing for you.

## Topics

### Getting and Setting the Control Type

func controlType() -> PDFWidgetControlType

Returns the type of the control.

func setControlType(PDFWidgetControlType)

Sets the type of the control.

### Getting and Setting the Control’s State

func state() -> Int

Returns the state of the control.

func setState(Int)

Sets the state of the control.

### Getting and Setting the Control’s Appearance

func backgroundColor() -> NSColor!

Returns the background color of the control.

func setBackgroundColor(NSColor!)

Sets the control’s background color.

### Getting and Setting the Control Label Font Attributes

func font() -> NSFont!

Returns the font used in the control’s label.

func setFont(NSFont!)

Sets the font of the control’s label.

func fontColor() -> NSColor!

Returns the font color used in the control’s label.

func setFontColor(NSColor!)

Sets the font color used in the control’s label.

### Getting and Setting the Control Label Text

func caption() -> String!

Returns the text of the label on a push button control.

func setCaption(String!)

Sets the text of the label on a push button control.

### Managing Radio Button Behavior

func allowsToggleToOff() -> Bool

Returns a Boolean value indicating whether a radio button behaves in a toggling manner.

### Managing Control State Values and Form Fields

func onStateValue() -> String!

Returns the string associated with the on state of a radio button or checkbox control.

func setOnStateValue(String!)

Sets the string that is associated with the on state of a radio button or checkbox control.

func fieldName() -> String!

Returns the internal name of a field (used for reset-form actions).

func setFieldName(String!)

Sets the internal name of a field (used for reset-form actions).

### Constants

enum PDFWidgetControlType

The types of annotation buttons.

### Instance Methods

func setAllowsToggleToOff(Bool)

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

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

