

- PDFKit
-  PDFAppearanceCharacteristics 

Class

# PDFAppearanceCharacteristics

An object that represents appearance characteristics of a widget annotation.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
class PDFAppearanceCharacteristics
```

## Topics

### Configuring a Widget’s Appearance

var backgroundColor: UIColor?

The background color of the widget annotation.

var borderColor: UIColor?

The border color of the widget annotation.

var caption: String?

The text that the button widget annotation displays when the user isn’t interacting with it.

var controlType: PDFWidgetControlType

The type of button widget annotation.

var downCaption: String?

The text that the button widget annotation displays when the user holds down on it.

var rolloverCaption: String?

The text that the widget annotation displays when the user hovers the pointer over it.

var rotation: Int

The number of degrees, in multiples of 90, that the widget annotation rotates counterclockwise relative to the page.

var appearanceCharacteristicsKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the appearance characteristic key-value pairs.

struct PDFAppearanceCharacteristicsKey

Keys to control a widget’s appearance.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCopying
- NSObjectProtocol

## See Also

### Configuring Widget Annotations

var widgetFieldType: PDFAnnotationWidgetSubtype

The type of widget annotation, such as button, choice, or text.

var widgetStringValue: String?

The string value of the widget annotation.

var widgetDefaultStringValue: String?

The string value that the widget reverts to when performing a reset form action.

var fieldName: String?

The widget identifier for form annotation actions and behaviors.

var backgroundColor: UIColor?

The color of the widget’s background.

var isReadOnly: Bool

A Boolean value that determines whether the widget is editable.

enum PDFWidgetControlType

The types of annotation buttons.

