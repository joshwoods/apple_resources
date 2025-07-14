

- PDFKit
-  PDFAnnotationText Deprecated

Class

# PDFAnnotationText

A `PDFAnnotationText` object displays as an icon (such as a “sticky note”) attached to a specified point in the PDF document.

macOS 10.4–10.12Deprecated

``` source
class PDFAnnotationText
```

Deprecated

Use PDFAnnotationSubtype instead.

## Overview

Each `PDFAnnotationText` object has a `PDFAnnotationPopup` object associated with it. In its closed state, the annotation appears as an icon. In its open state, it displays as a pop-up window containing the text of the note. Note that your application must do the work to put up a window containing the text in response to a PDFViewAnnotationHitNotification. Currently, text annotations do not scale and rotate with the page.

## Topics

### Managing the Annotation Icon’s Type

func iconType() -> PDFTextAnnotationIconType

Returns the icon type for the annotation.

func setIconType(PDFTextAnnotationIconType)

Sets the icon type for the annotation.

### Constants

enum PDFTextAnnotationIconType

The types of icons that a text annotation can use.

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

class PDFAnnotationTextWidget

A `PDFAnnotationTextWidget` object allows you to manage the appearance and content of text fields.

Deprecated

