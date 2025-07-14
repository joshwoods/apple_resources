

- PDFKit
-  PDFAnnotationKey 

Structure

# PDFAnnotationKey

Keys for setting properties of annotations.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
struct PDFAnnotationKey
```

## Topics

### Configuring General Properties

static let contents: PDFAnnotationKey

The text that the annotation displays or represents.

static let date: PDFAnnotationKey

The date, or string representation of a date, of the annotation’s most recent modification.

static let flags: PDFAnnotationKey

An integer value that specifies flags for the annotation.

static let name: PDFAnnotationKey

A string that uniquely identifies the annotation among all annotations on the same page.

static let page: PDFAnnotationKey

A dictionary or PDF page object that includes the annotation.

static let parent: PDFAnnotationKey

A dictionary or annotation object that a pop-up or widget belongs to.

static let quadPoints: PDFAnnotationKey

An array of floating point values that specifies a rectangular region of a page.

static let rect: PDFAnnotationKey

The rectangle that the annotation occupies on the page, in page-space coordinates.

static let subtype: PDFAnnotationKey

The type of annotation that the entries in a dictionary describe.

static let textLabel: PDFAnnotationKey

A string that represents the title of the annotation.

### Configuring Annotation Appearance

static let appearanceDictionary: PDFAnnotationKey

A dictionary that contains properties for controlling the annotation’s visual appearance.

static let appearanceState: PDFAnnotationKey

A string that specifies the appearance stream for the annotation.

static let border: PDFAnnotationKey

An array of integers or border objects that describes the border of the annotation.

static let borderStyle: PDFAnnotationKey

A dictionary that contains the properties of the annotation’s border.

static let color: PDFAnnotationKey

An array of floats or a color object that specifies the annotation’s color.

static let defaultAppearance: PDFAnnotationKey

A string value a free text annotation uses to format the text.

static let highlightingMode: PDFAnnotationKey

A string value that defines the way an annotation highlights when the user activates it, such as when clicking or tapping a link.

struct PDFAnnotationHighlightingMode

static let iconName: PDFAnnotationKey

A string value that specifies the name of an icon for a text or stamp annotation.

static let interiorColor: PDFAnnotationKey

An array of floating point values or a PDF color object that annotations use to fill interior space, such as line endings, squares, or circles.

static let quadding: PDFAnnotationKey

An integer value that specifies left, right, or center justification.

### Configuring Line Properties

static let lineEndingStyles: PDFAnnotationKey

An array of string values that specifies the styles to use for the ends of lines.

enum PDFLineStyle

The following constants specify the available line ending styles.

static let linePoints: PDFAnnotationKey

An array of floating point values that specifies the starting and ending points, in page-space coordinates, of a line.

struct PDFAnnotationLineEndingStyle

### Configuring Pop-Up Annotations

static let popup: PDFAnnotationKey

A dictionary or annotation object that specifies the annotation to pop up for text entry or editing.

static let open: PDFAnnotationKey

A Boolean value that specifies whether the pop-up is in an opened state, showing its text content, or in a closed state and showing an icon.

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

struct PDFAnnotationWidgetSubtype

### Configuring Actions

static let destination: PDFAnnotationKey

An array, name, or string that represents the destination of an action.

static let action: PDFAnnotationKey

A dictionary or PDF action object that represents an action to take, such as when the user clicks or taps a button.

static let additionalActions: PDFAnnotationKey

A dictionary or PDF action object that represents additional actions an annotation can perform, such as when it receives input focus.

### Configuring Ink Annotations

static let inklist: PDFAnnotationKey

An array of arrays that represents stroked paths.

### Creating an Annotation Key

init(rawValue: String)

Creates an annotation key using the specified raw string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Modifying Annotation Attributes

var annotationKeyValues: [AnyHashable : Any]

A dictionary that contains a deep copy of the widget’s properties.

func value(forAnnotationKey: PDFAnnotationKey) -> Any?

Returns a deep copy of the key-value pairs of properties for the specified key.

func setValue(Any, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a value in the annotation’s dictionary.

func setBoolean(Bool, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a Boolean value in the annotation’s dictionary.

func setRect(CGRect, forAnnotationKey: PDFAnnotationKey) -> Bool

Sets a rectangle value in the annotation’s dictionary.

func removeValue(forAnnotationKey: PDFAnnotationKey)

Removes a value from the annotation’s dictionary.

