

- AppKit
-  NSSliderTouchBarItem 

Class

# NSSliderTouchBarItem

A bar item that provides a slider control for choosing a value in a range.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
class NSSliderTouchBarItem
```

## Topics

### Configuring the slider

var slider: NSSlider

The slider displayed by the bar item.

var label: String?

The text displayed alongside the slider.

var view: any NSView &amp; NSUserInterfaceCompression

### Configuring slider accessories

var minimumValueAccessory: NSSliderAccessory?

The accessory that appears at the end of the slider with the minimum value.

var maximumValueAccessory: NSSliderAccessory?

The accessory that appears at the end of the slider with the maximum value.

var valueAccessoryWidth: NSSliderAccessory.Width

The width of the value accessories that appear at either end of the slider.

### Managing the slider’s value

var minimumSliderWidth: CGFloat

The minimum width of the slider’s track.

var maximumSliderWidth: CGFloat

The maximum width of the slider’s track.

var doubleValue: Double

The double value of the slider.

### Handling slider interaction

var target: AnyObject?

An object that is notified when a user interacts with the slider or either of the accessories.

var action: Selector?

The selector on the target object that is invoked when a user interacts with the slider or either of the accessories.

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

class NSPopoverTouchBarItem

A bar item that provides a two-state control that can expand into its second state, showing the contents of a bar that it owns.

class NSSharingServicePickerTouchBarItem

A bar item that, along with its delegate, provides a list of objects eligible for sharing.

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

