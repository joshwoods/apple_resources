

- AppKit
- NSButton
-  isSpringLoaded 

Instance Property

# isSpringLoaded

A Boolean value that indicates whether spring loading is enabled for the button.

macOS 10.10.3+

``` source
@MainActor
var isSpringLoaded: Bool { get set }
```

## Discussion

The value of this property is true if spring loading is enabled for the button, and false if it is not. The default is false.

On pressure-sensitive systems, such as systems with the Force Touch trackpad, spring loading is a feature that allows a user to activate a button by dragging selected items over it and force clicking—pressing harder—without dropping the selected items. The user can then continue dragging the items, possibly to perform additional actions.

A practical example of this feature can be found in the Calendar app. A selected calendar event can be dragged over the Calendars button in the toolbar. Force clicking on the button displays the calendar list without releasing the selected event. The event can then be dropped onto a calendar in the list, which assigns it to that calendar.

If spring loading is enabled on a button and a user drags items over it, the button highlights to indicate that it responds to force clicking. If the user presses harder, additional highlighting occurs to indicate that the button was fully activated.

On systems that don’t support pressure sensitivity, simply hovering over the button for a short period of time is sufficient to activate the button.

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

var attributedTitle: NSAttributedString

The title that the button displays in an off state, as an attributed string.

var attributedAlternateTitle: NSAttributedString

The title that the button displays as an attributed string when the button is in an on state.

var title: String

The title displayed on the button when it’s in an off state.

var symbolConfiguration: NSImage.SymbolConfiguration?

The combination of point size, weight, and scale to use when sizing and displaying symbol images.

var sound: NSSound?

The sound that plays when the user clicks the button.

var maxAcceleratorLevel: Int

An integer value indicating the maximum pressure level for a button of type NSMultiLevelAcceleratorButton.

