

- AppKit
-  NSPopoverTouchBarItem 

Class

# NSPopoverTouchBarItem

A bar item that provides a two-state control that can expand into its second state, showing the contents of a bar that it owns.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
class NSPopoverTouchBarItem
```

## Topics

### Configuring the collapsed popover

var collapsedRepresentation: NSView

The view displayed when this item is displayed in its parent bar.

var collapsedRepresentationImage: UIImage?

The image displayed by the button for the default collapsed representation.

var collapsedRepresentationLabel: String

The localized string displayed by the button for the default collapsed representation.

### Configuring the expanded popover

var popoverTouchBar: NSTouchBar

The bar displayed when this item is “popped.”

var showsCloseButton: Bool

A Boolean value that determines whether a close button should be shown on the popover bar.

var pressAndHoldTouchBar: NSTouchBar?

The bar that is displayed when a user press-and-holds on the popover item.

### Expanding and collapsing a popover

func showPopover(Any?)

Replaces the main bar with this item’s popover bar.

func dismissPopover(Any?)

Restores the previously visible main bar.

func makeStandardActivatePopoverGestureRecognizer() -> NSGestureRecognizer

Returns a gesture recognizer, configured to invoke the showPopover(_:) method.

### Configuring bar customization

var customizationLabel: String!

The user-visible string identifying this item during bar customization.

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

class NSSharingServicePickerTouchBarItem

A bar item that, along with its delegate, provides a list of objects eligible for sharing.

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

