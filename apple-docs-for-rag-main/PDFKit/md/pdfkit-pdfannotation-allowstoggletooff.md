

- PDFKit
- PDFAnnotation
-  allowsToggleToOff 

Instance Property

# allowsToggleToOff

A Boolean value that indicates whether clicking or tapping a selected radio button toggles it to an unselected state.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
var allowsToggleToOff: Bool { get set }
```

## Discussion

To implement a group of radio buttons where at least one option must remain in a selected state, set allowsToggleToOff to false on each button in the group.

## See Also

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

var radiosInUnison: Bool

A Boolean value that indicates whether radio buttons in a group turn on and off in unison.

