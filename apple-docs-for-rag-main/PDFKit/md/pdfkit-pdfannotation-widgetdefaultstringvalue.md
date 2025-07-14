

- PDFKit
- PDFAnnotation
-  widgetDefaultStringValue 

Instance Property

# widgetDefaultStringValue

The string value that the widget reverts to when performing a reset form action.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
var widgetDefaultStringValue: String? { get set }
```

## Discussion

For text and choice widgets, this property specifies the string value that a reset form action sets on a widget.

For radio buttons and checkboxes, set this property to `Off` if the desired default is for the button to be in an unselected state; otherwise, set it to the buttonWidgetStateString.

## See Also

### Configuring Widget Annotations

var widgetFieldType: PDFAnnotationWidgetSubtype

The type of widget annotation, such as button, choice, or text.

var widgetStringValue: String?

The string value of the widget annotation.

var fieldName: String?

The widget identifier for form annotation actions and behaviors.

var backgroundColor: UIColor?

The color of the widget’s background.

var isReadOnly: Bool

A Boolean value that determines whether the widget is editable.

enum PDFWidgetControlType

The types of annotation buttons.

class PDFAppearanceCharacteristics

An object that represents appearance characteristics of a widget annotation.

