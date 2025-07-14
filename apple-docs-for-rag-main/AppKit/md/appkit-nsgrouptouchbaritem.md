

- AppKit
-  NSGroupTouchBarItem 

Class

# NSGroupTouchBarItem

A bar item that provides a bar to contain other items.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
class NSGroupTouchBarItem
```

## Topics

### Creating a group

convenience init(identifier: NSTouchBarItem.Identifier, items: [NSTouchBarItem])

Initializes and returns a group item whose bar is constructed from the supplied items.

convenience init(identifier: NSTouchBarItem.Identifier, items: [NSTouchBarItem], allowedCompressionOptions: NSUserInterfaceCompressionOptions)

Initializes and returns a group item whose bar is constructed from the supplied items, and with the specified compression options.

convenience init(alertStyleWithIdentifier: NSTouchBarItem.Identifier)

Initializes and returns a group item configured to match system alerts.

### Configuring groups

var groupTouchBar: NSTouchBar

A bar that holds this group’s items.

var groupUserInterfaceLayoutDirection: NSUserInterfaceLayoutDirection

The user interface direction that controls the layout order of the items.

### Configuring item width

var prefersEqualWidths: Bool

A Boolean value that specifies that items should have equal widths when possible.

var preferredItemWidth: CGFloat

The preferred width for items in the group when prefersEqualWidths is true.

### Configuring item compression

var effectiveCompressionOptions: NSUserInterfaceCompressionOptions

The compression options that are currently active on the group.

var prioritizedCompressionOptions: [NSUserInterfaceCompressionOptions]

The allowed compression options, in the order they should be applied.

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

class NSButtonTouchBarItem

A bar item that provides a button.

class NSPickerTouchBarItem

A bar item that provides a picker control with multiple options.

enum ControlRepresentation

Constants that specify display styles for picker bar items.

enum SelectionMode

Constants that specify selection modes for picker bar items.

