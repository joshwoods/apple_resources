

- PDFKit
-  PDFAnnotation 

Class

# PDFAnnotation

An annotation in a PDF document.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.4+tvOS 11.0+visionOS 1.0+

``` source
class PDFAnnotation
```

## Mentioned in 

Adding Custom Graphics to a PDF

Adding Widgets to a PDF Document

## Overview

In addition to its primary textual content, a PDF file can contain annotations that represent links, form elements, highlighting circles, textual notes, and so on. Each annotation has a specific location on a page and may offer interactivity with the user.

## Topics

### Creating an Annotation

init(bounds: CGRect, forType: PDFAnnotationSubtype, withProperties: [AnyHashable : Any]?)

Creates a PDF annotation with the specified bounds, type, and optional properties.

struct PDFAnnotationSubtype

The type of annotation, such as circle, text, or ink.

### Accessing Information About an Annotation

var page: PDFPage?

Returns the page that the annotation is associated with.

var modificationDate: Date?

Returns the modification date of the annotation.

var userName: String?

Returns the name of the user who created the annotation.

var type: String?

Returns the type of the annotation.

var action: PDFAction?

An object that represents an action for a PDF element, such as a link annotation.

class PDFAction

An action that is performed when, for example, a PDF annotation is activated or an outline item is clicked.

class PDFDestination

A `PDFDestination` object describes a point on a PDF page.

### Managing Annotation Drawing and Output

func draw(with: PDFDisplayBox, in: CGContext)

Draws the annotation in a graphics context using page-space coordinates relative to the origin of the specified box.

var shouldDisplay: Bool

Returns a Boolean value indicating whether the annotation should be displayed.

var shouldPrint: Bool

Returns a Boolean value indicating whether the annotation should appear when the document is printed.

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

struct PDFAnnotationKey

Keys for setting properties of annotations.

### Managing Annotation Display Characteristics

var alignment: NSTextAlignment

The alignment of the free text and text widget annotation’s text content.

var bounds: CGRect

Returns the bounding box for the annotation in page space.

var contents: String?

Returns the textual content (if any) associated with the annotation.

var font: UIFont?

The font the annotation uses to display text.

var fontColor: UIColor?

The font color the annotation uses to display text.

var border: PDFBorder?

Sets the border style for the annotation.

class PDFBorder

An optional border for an annotation that lies completely within the annotation rectangle.

var isHighlighted: Bool

A Boolean value that indicates whether the annotation is in a highlighted state, such as when the mouse is down on a link annotation.

var color: UIColor

Sets the stroke color for the annotation.

var hasAppearanceStream: Bool

Returns a Boolean value that indicates whether the annotation has an appearance stream associated with it.

### Configuring Shape Annotations

var interiorColor: UIColor?

The fill color for drawing a circle, line, or square annotation.

### Configuring Line Annotations

var startPoint: CGPoint

The point where a line begins, in annotation-space coordinates.

var endPoint: CGPoint

The point where a line ends, in annotation-space coordinates.

var startLineStyle: PDFLineStyle

The style of the line annotation’s starting point, such as square or filled arrowhead.

var endLineStyle: PDFLineStyle

The style of the line annotation’s ending point, such as square or filled arrowhead.

class func lineStyle(fromName: String) -> PDFLineStyle

Returns a line style that corresponds to the specified name.

class func name(for: PDFLineStyle) -> String

Returns the name of the line style, which matches the definition in the Adobe PDF Specification.

### Configuring Link Annotations

var destination: PDFDestination?

The destination for a link annotation.

var url: URL?

A URL for a link annotation.

### Configuring Text Annotations

var iconType: PDFTextAnnotationIconType

The type of icon to display for a pop-up text annotation.

enum PDFTextAnnotationIconType

The types of icons that a text annotation can use.

struct PDFAnnotationTextIconType

Constants for icon type values in text annotation property dictionaries.

### Configuring Pop-Up Annotations

var popup: PDFAnnotation?

Returns the pop-up annotation associated with an annotation.

var isOpen: Bool

A Boolean value that indicates whether the pop-up annotation is in an opened state, displaying its text content, or in a closed state, displaying an icon.

### Configuring Text Markup Annotations

var markupType: PDFMarkupType

The markup type that the annotation displays, either highlight, strikethrough, underline, or redact.

enum PDFMarkupType

The styles available for markup annotations in PDFKit.

var quadrilateralPoints: [NSValue]?

An array of values that represents the points bounding the marked-up text.

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

class PDFAppearanceCharacteristics

An object that represents appearance characteristics of a widget annotation.

### Configuring Text Widget Annotations

var isMultiline: Bool

A Boolean value that indicates whether the text widget annotation displays multiple lines.

var isPasswordField: Bool

A Boolean value that indicates whether the text widget annotation displays a password field using bullet characters.

var maximumLength: Int

The maximum number of characters the text widget annotation allows.

var hasComb: Bool

A Boolean value that indicates whether the annotation divides the text widget’s bounds into equally spaced segments, such as in a form entry field.

### Configuring Button Widget Annotations

var widgetControlType: PDFWidgetControlType

The type of button widget control, either radio button, push button, or checkbox.

var buttonWidgetState: PDFWidgetCellState

The current state of the button widget annotation.

enum PDFWidgetCellState

The state of a button annotation, either on, off, or mixed.

var buttonWidgetStateString: String

A string value that differentiates button widgets in the same group, such as to identify mutually exclusive radio buttons from each other.

var caption: String?

The title of push button widget annotations.

var allowsToggleToOff: Bool

A Boolean value that indicates whether clicking or tapping a selected radio button toggles it to an unselected state.

var radiosInUnison: Bool

A Boolean value that indicates whether radio buttons in a group turn on and off in unison.

### Configuring Choice Widget Annotations

var choices: [String]?

An array of strings that specifies the options in either a list or a pop-up menu.

var isListChoice: Bool

A Boolean value that indicates whether the choice widget annotation is a list or a pop-up menu.

var values: [String]?

An array of strings that specifies the export values for items in a list or a pop-up menu.

### Configuring Ink Annotations

var paths: [UIBezierPath]?

An array of bezier paths, in annotation-space coordinates, that compose the annotation.

func add(UIBezierPath)

Adds a bezier path to the ink annotation.

func remove(UIBezierPath)

Removes a bezier path from an ink annotation.

### Configuring Stamp Annotations

var stampName: String?

The name of the stamp, a text or graphics annotation that emulates a rubber stamp effect.

### Deprecated

Deprecated Symbols

Review unsupported symbols and their replacements.

### Instance Properties

var isActivatableTextField: Bool

## Relationships

### Inherits From

- NSObject

### Inherited By

- PDFAnnotationButtonWidget
- PDFAnnotationChoiceWidget
- PDFAnnotationCircle
- PDFAnnotationFreeText
- PDFAnnotationInk
- PDFAnnotationLine
- PDFAnnotationLink
- PDFAnnotationMarkup
- PDFAnnotationPopup
- PDFAnnotationSquare
- PDFAnnotationStamp
- PDFAnnotationText
- PDFAnnotationTextWidget

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

### Annotations

Adding Widgets to a PDF Document

Add text, button, and choice widgets to a PDF document.

Adding Custom Graphics to a PDF

Create and add custom annotation and page graphics to your PDF document.

Custom Graphics

Demonstrates adding a watermark to a PDF page.

PDF Widgets

Demonstrates adding widgets—interactive form elements—to a PDF document.

