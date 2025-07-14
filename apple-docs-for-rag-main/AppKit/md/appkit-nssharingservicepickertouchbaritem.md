

- AppKit
-  NSSharingServicePickerTouchBarItem 

Class

# NSSharingServicePickerTouchBarItem

A bar item that, along with its delegate, provides a list of objects eligible for sharing.

iOS 10.13+iPadOS 10.13+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
class NSSharingServicePickerTouchBarItem
```

## Topics

### Setting the delegate

var delegate: (any NSSharingServicePickerTouchBarItemDelegate)?

The object that acts as the delegate of the sharing service picker bar item.

protocol NSSharingServicePickerTouchBarItemDelegate

A protocol that a sharing service picker item delegate uses to provide a list of items eligible for sharing.

### Configuring the appearance

var buttonImage: NSImage?

The image displayed in the sharing service picker item button.

var buttonTitle: String

The text displayed in the sharing service picker item button.

### Enabling the item

var isEnabled: Bool

A Boolean value that specifies whether the sharing service picker item is enabled.

### Supporting sharing

var activityItemsConfiguration: (any UIActivityItemsConfigurationReading)?

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

class NSSliderTouchBarItem

A bar item that provides a slider control for choosing a value in a range.

class NSStepperTouchBarItem

A bar item that provides a stepper control for incrementing or decrementing a value.

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

