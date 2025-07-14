

- PDFKit
-  PDFWidgetControlType 

Enumeration

# PDFWidgetControlType

The types of annotation buttons.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
enum PDFWidgetControlType
```

## Topics

### Constants

case unknownControl

Unknown control type.

case pushButtonControl

Push button control.

case radioButtonControl

Radio button control.

case checkBoxControl

Check box control.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

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

class PDFAppearanceCharacteristics

An object that represents appearance characteristics of a widget annotation.

