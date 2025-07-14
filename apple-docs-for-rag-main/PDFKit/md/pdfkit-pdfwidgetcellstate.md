

- PDFKit
-  PDFWidgetCellState 

Enumeration

# PDFWidgetCellState

The state of a button annotation, either on, off, or mixed.

iOS 11.0+iPadOS 11.0+Mac Catalyst 11.0+macOS 10.4+tvOSvisionOS 1.0+

``` source
enum PDFWidgetCellState
```

## Topics

### Choosing a Cell State

case onState

The button widget is in a selected state.

case offState

The button widget is in an unselected state.

case mixedState

The button widget is in a mixed state, neither on nor off.

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

### Configuring Button Widget Annotations

var widgetControlType: PDFWidgetControlType

The type of button widget control, either radio button, push button, or checkbox.

var buttonWidgetState: PDFWidgetCellState

The current state of the button widget annotation.

var buttonWidgetStateString: String

A string value that differentiates button widgets in the same group, such as to identify mutually exclusive radio buttons from each other.

var caption: String?

The title of push button widget annotations.

var allowsToggleToOff: Bool

A Boolean value that indicates whether clicking or tapping a selected radio button toggles it to an unselected state.

var radiosInUnison: Bool

A Boolean value that indicates whether radio buttons in a group turn on and off in unison.

