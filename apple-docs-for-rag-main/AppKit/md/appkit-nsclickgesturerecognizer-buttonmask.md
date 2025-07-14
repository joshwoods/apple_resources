

- AppKit
- NSClickGestureRecognizer
-  buttonMask 

Instance Property

# buttonMask

A bit mask of the button (or buttons) required to recognize this click.

macOS 10.10+

``` source
@MainActor
var buttonMask: Int { get set }
```

## Discussion

Bit `0` represents the primary button, bit `1` is the secondary button, and so on. So to track clicks of the secondary button, assign the value `0x2` (which corresponds to a `1` in bit `1`) to this property. The default value of this property is `0x1`, which detects clicks in the primary mouse button.

Changing the value of this property also sets the values of the delaysPrimaryMouseButtonEvents, delaysSecondaryMouseButtonEvents, and delaysOtherMouseButtonEvents properties to true for each of the buttons you specified.

## See Also

### Configuring the Gesture

var numberOfClicksRequired: Int

The number of clicks required to match.

var numberOfTouchesRequired: Int

The number of touches required in an NSTouchBar object for the gesture recognizer to match.

