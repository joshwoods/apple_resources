

- AppKit
- NSClickGestureRecognizer
-  numberOfClicksRequired 

Instance Property

# numberOfClicksRequired

The number of clicks required to match.

macOS 10.10+

``` source
@MainActor
var numberOfClicksRequired: Int { get set }
```

## Discussion

The value in this property should always be a positive integer. Negative integers or `0` cause this object to never recognize its gesture. The default value of this property is `1`.

## See Also

### Configuring the Gesture

var buttonMask: Int

A bit mask of the button (or buttons) required to recognize this click.

var numberOfTouchesRequired: Int

The number of touches required in an NSTouchBar object for the gesture recognizer to match.

