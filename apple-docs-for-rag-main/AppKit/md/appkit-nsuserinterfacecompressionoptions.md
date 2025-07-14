

- AppKit
-  NSUserInterfaceCompressionOptions 

Class

# NSUserInterfaceCompressionOptions

An object that specifies how user interface elements resize themselves when space is constrained.

macOS 10.13+

``` source
class NSUserInterfaceCompressionOptions
```

## Overview

An instance of NSUserInterfaceCompressionOptions contains zero or more options. Because a compression options object behaves like a set, you can use common operations like intersection, union and subtraction to interact with instances and their members.

You can access system-defined options through the class methods detailed in Creating standard options, or you can create your own custom options with the init(identifier:) initializer.

To compare two different compression options objects, use the methods described in the Comparing compression options section.

## Topics

### Creating a compression option

init()

Creates an option object containing no options.

init(options: Set&lt;NSUserInterfaceCompressionOptions>)

Creates an option object that represents the union of the supplied options.

init(identifier: String)

Creates an option object with the given identifier string.

init(coder: NSCoder)

Creates an option object from data in an unarchiver.

### Creating standard options

class var hideImages: NSUserInterfaceCompressionOptions

An option specifying that views should hide their images.

class var hideText: NSUserInterfaceCompressionOptions

An option specifying that views should hide their text.

class var reduceMetrics: NSUserInterfaceCompressionOptions

An option specifying that views should reduce their internal metrics.

class var breakEqualWidths: NSUserInterfaceCompressionOptions

An option specifying that views should no longer maintain equal width constraints.

class var standardOptions: NSUserInterfaceCompressionOptions

An option that represents the union of all standard compression options.

### Comparing compression options

var isEmpty: Bool

A Boolean value that denotes whether the option is empty.

func contains(NSUserInterfaceCompressionOptions) -> Bool

Determines whether the supplied compression options are all present in the current instance.

func intersects(NSUserInterfaceCompressionOptions) -> Bool

Determines whether the supplied compression options intersect with the current instance’s options.

### Combining compression options

func union(NSUserInterfaceCompressionOptions) -> NSUserInterfaceCompressionOptions

Creates a new compression options object representing the union with the provided options.

func subtracting(NSUserInterfaceCompressionOptions) -> NSUserInterfaceCompressionOptions

Creates a new compression options object with the supplied options removed.

## Relationships

### Inherits From

- NSObject

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

class NSButtonTouchBarItem

A bar item that provides a button.

class NSPickerTouchBarItem

A bar item that provides a picker control with multiple options.

enum ControlRepresentation

Constants that specify display styles for picker bar items.

enum SelectionMode

Constants that specify selection modes for picker bar items.

