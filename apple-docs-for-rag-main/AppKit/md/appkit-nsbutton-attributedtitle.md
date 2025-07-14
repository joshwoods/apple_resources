

- AppKit
- NSButton
-  attributedTitle 

Instance Property

# attributedTitle

The title that the button displays in an off state, as an attributed string.

macOS

``` source
@NSCopying @MainActor
var attributedTitle: NSAttributedString { get set }
```

## Discussion

This property contains an string of class `NSAttributedString`, which appears on the button when the button is in an off state. If the button doesn’t display a title, then this property contains an empty attributed string.

A button’s title is always displayed if the button doesn’t use its alternate contents for highlighting or displaying the on state. By default, a button’s title is Button.

## See Also

### Configuring Buttons

func setButtonType(NSButton.ButtonType)

Sets the button’s type, which affects its user interface and behavior when clicked.

func getPeriodicDelay(UnsafeMutablePointer&lt;Float>, interval: UnsafeMutablePointer&lt;Float>)

Returns by reference the delay and interval periods for a continuous button.

func setPeriodicDelay(Float, interval: Float)

Sets the message delay and interval periods for a continuous button.

var contentTintColor: NSColor?

A tint color to use for the template image and text content.

var hasDestructiveAction: Bool

A Boolean value that defines whether a button’s action has a destructive effect.

var alternateTitle: String

The title that the button displays when the button is in an on state.

var attributedAlternateTitle: NSAttributedString

The title that the button displays as an attributed string when the button is in an on state.

var title: String

The title displayed on the button when it’s in an off state.

var symbolConfiguration: NSImage.SymbolConfiguration?

The combination of point size, weight, and scale to use when sizing and displaying symbol images.

var sound: NSSound?

The sound that plays when the user clicks the button.

var isSpringLoaded: Bool

A Boolean value that indicates whether spring loading is enabled for the button.

var maxAcceleratorLevel: Int

An integer value indicating the maximum pressure level for a button of type NSMultiLevelAcceleratorButton.

