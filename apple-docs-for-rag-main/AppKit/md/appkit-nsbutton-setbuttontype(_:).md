

- AppKit
- NSButton
-  setButtonType(\_:) 

Instance Method

# setButtonType(\_:)

Sets the button’s type, which affects its user interface and behavior when clicked.

macOS

``` source
@MainActor
func setButtonType(_ type: NSButton.ButtonType)
```

## Parameters 

`type`  

A constant specifying the type of the button. The available button types are listed under NSButton.ButtonType in the NSButtonCell class.

## Discussion

This method causes the button to update to reflect the new type before the method finishes executing.

The types available are for the most common button types, which are also accessible in Interface Builder. You can configure different behavior with the `NSButtonCell` methods highlightsBy and showsStateBy.

Note that there is no `-buttonType` method. The set method sets various button properties that together establish the behavior of the type.

## See Also

### Related Documentation

var image: NSImage?

The image that appears on the button when it’s in an off state, or `nil` if there is no such image.

func setButtonType(NSButton.ButtonType)

Sets how the button highlights while pressed and how it shows its state.

Button Programming Topics

var alternateImage: NSImage?

An alternate image that appears on the button when the button is in an on state.

### Configuring Buttons

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

var isSpringLoaded: Bool

A Boolean value that indicates whether spring loading is enabled for the button.

var maxAcceleratorLevel: Int

An integer value indicating the maximum pressure level for a button of type NSMultiLevelAcceleratorButton.

