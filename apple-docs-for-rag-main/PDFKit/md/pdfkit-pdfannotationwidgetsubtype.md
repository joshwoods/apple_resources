

- PDFKit
-  PDFAnnotationWidgetSubtype 

Structure

# PDFAnnotationWidgetSubtype

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAnnotationWidgetSubtype
```

## Mentioned in 

Adding Widgets to a PDF Document

## Topics

### Configuring a Widget Subtype

static let button: PDFAnnotationWidgetSubtype

A button widget type, including push buttons, checkboxes, and radio buttons.

static let choice: PDFAnnotationWidgetSubtype

A type that presents a list of choices the user can choose from.

static let signature: PDFAnnotationWidgetSubtype

A digital signature widget type.

static let text: PDFAnnotationWidgetSubtype

A text field the user can type text in.

### Creating a Widget Subtype

init(rawValue: String)

Creates a widget subtype using the specified raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Configuring Widget Annotations

static let widgetAppearanceDictionary: PDFAnnotationKey

A dictionary or appearance characteristic object that contains properties for controlling the widget’s visual appearance.

static let widgetBackgroundColor: PDFAnnotationKey

An array of floating point values or a PDF color object that specifies the widget’s background color.

static let widgetBorderColor: PDFAnnotationKey

An array of floating point values or a PDF color object that specifies the widget’s border color.

static let widgetCaption: PDFAnnotationKey

A string that a push button widget displays when it isn’t in a pressed state.

static let widgetDefaultValue: PDFAnnotationKey

A default value for the widget.

static let widgetDownCaption: PDFAnnotationKey

A string that a push button widgets displays when it’s in a pressed state.

static let widgetFieldFlags: PDFAnnotationKey

An integer value that specifies flags for a widget.

static let widgetFieldType: PDFAnnotationKey

A string that specifies the type of widget, such as button, checkbox, or signature field.

static let widgetMaxLen: PDFAnnotationKey

An integer value that specifies the maximum length of a text field, in characters.

static let widgetOptions: PDFAnnotationKey

An array that specifies the options to present in radio buttons or choice lists.

static let widgetRolloverCaption: PDFAnnotationKey

A string that push button widgets display when the pointer is over the button, but not clicking it.

static let widgetRotation: PDFAnnotationKey

An integer value that specifies the rotation of the widget.

static let widgetTextLabelUI: PDFAnnotationKey

A user-visible alternative field name that identifies the widget, typically for accessibility purposes.

static let widgetValue: PDFAnnotationKey

The widget’s value, typically for text and choice widgets.

