

- WatchKit
- WKLongPressGestureRecognizer
-  numberOfTapsRequired 

Instance Property

# numberOfTapsRequired

The number of taps on the interface object that are required for the gesture to be recognized.

watchOS 3.0+

``` source
var numberOfTapsRequired: Int { get set }
```

## Discussion

The default value of this property is `1`, but you can change this value when configuring the gesture recognizer in Interface Builder.

## See Also

### Configuring the Gesture Recognizer

var minimumPressDuration: CFTimeInterval

The minimum amount of time (in seconds) that the user’s fingers must be touching the interface object.

var allowableMovement: CGFloat

The maximum movement of the finger on the interface object that allows the gesture to be recognized.

