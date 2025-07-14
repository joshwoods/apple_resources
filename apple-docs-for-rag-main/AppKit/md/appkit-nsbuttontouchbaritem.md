

- AppKit
-  NSButtonTouchBarItem 

Class

# NSButtonTouchBarItem

A bar item that provides a button.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.15+

``` source
@MainActor
class NSButtonTouchBarItem
```

## Topics

### Creating a button item

convenience init(identifier: NSTouchBarItem.Identifier, image: UIImage, target: Any?, action: Selector?)

convenience init(identifier: NSTouchBarItem.Identifier, title: String, image: UIImage, target: Any?, action: Selector?)

convenience init(identifier: NSTouchBarItem.Identifier, title: String, target: Any?, action: Selector?)

### Configuring button appearance

var title: String

var image: UIImage?

var bezelColor: UIColor?

### Configuring button state

var isEnabled: Bool

### Handling button interaction

var target: AnyObject?

var action: Selector?

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

class NSStepperTouchBarItem

A bar item that provides a stepper control for incrementing or decrementing a value.

class NSUserInterfaceCompressionOptions

An object that specifies how user interface elements resize themselves when space is constrained.

class NSPickerTouchBarItem

A bar item that provides a picker control with multiple options.

enum ControlRepresentation

Constants that specify display styles for picker bar items.

enum SelectionMode

Constants that specify selection modes for picker bar items.

