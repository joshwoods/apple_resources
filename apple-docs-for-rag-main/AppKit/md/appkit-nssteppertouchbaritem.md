

- AppKit
-  NSStepperTouchBarItem 

Class

# NSStepperTouchBarItem

A bar item that provides a stepper control for incrementing or decrementing a value.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
class NSStepperTouchBarItem
```

## Topics

### Creating a stepper item

convenience init(identifier: NSTouchBarItem.Identifier, drawingHandler: (NSRect, Double) -> Void)

convenience init(identifier: NSTouchBarItem.Identifier, formatter: Formatter)

### Handling stepper interaction

var target: AnyObject?

var action: Selector?

### Managing the stepper’s value

var value: Double

var maxValue: Double

var minValue: Double

var increment: Double

### Configuring bar customization

var customizationLabel: String!

## Relationships

### Inherits From

- NSTouchBarItem

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- Sendable

## See Also

### Touch Bar items

class NSTouchBarItem

A UI control shown in the Touch Bar on supported models of MacBook Pro.

class NSCandidateListTouchBarItem

A bar item that, along with its delegate, provides a list of textual suggestions for the current text view.

class NSColorPickerTouchBarItem

A bar item that provides a system-defined color picker.

class NSCustomTouchBarItem

A bar item that contains a responder of your choice, such as a view, a button, or a scrubber.

class NSGroupTouchBarItem

A bar item that provides a bar to contain other items.

class NSPopoverTouchBarItem

A bar item that provides a two-state control that can expand into its second state, showing the contents of a bar that it owns.

class NSSharingServicePickerTouchBarItem

A bar item that, along with its delegate, provides a list of objects eligible for sharing.

class NSSliderTouchBarItem

A bar item that provides a slider control for choosing a value in a range.

class NSUserInterfaceCompressionOptions

An object that specifies how user interface elements resize themselves when space is constrained.

class NSButtonTouchBarItem

A bar item that provides a button.

class NSPickerTouchBarItem

A bar item that provides a picker control with multiple options.

enum ControlRepresentation

Constants that specify display styles for picker bar items.

enum SelectionMode

Constants that specify selection modes for picker bar items.

