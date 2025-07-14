

- UIKit
- UITapGestureRecognizer
-  numberOfTouchesRequired 

Instance Property

# numberOfTouchesRequired

The number of fingers that the user must tap for gesture recognition.

iOS 3.2+iPadOS 3.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var numberOfTouchesRequired: Int { get set }
```

## Mentioned in 

Handling tap gestures

## Discussion

The default value is 1.

## See Also

### Configuring the gesture

var buttonMaskRequired: UIEvent.ButtonMask

The bit mask of the buttons the user must press for gesture recognition.

var numberOfTapsRequired: Int

The number of taps necessary for gesture recognition.

