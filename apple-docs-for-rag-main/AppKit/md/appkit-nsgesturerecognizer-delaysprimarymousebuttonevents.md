

- AppKit
- NSGestureRecognizer
-  delaysPrimaryMouseButtonEvents 

Instance Property

# delaysPrimaryMouseButtonEvents

A Boolean value that indicates whether primary mouse button events are delivered only after gesture recognition fails.

macOS 10.10+

``` source
@MainActor
var delaysPrimaryMouseButtonEvents: Bool { get set }
```

## Discussion

When the value of this property is true, primary mouse button events are delivered to the target view only after gesture recognition fails. Set this property to true to prevent the view from processing events that might be recognized as part of a gesture. Once gesture recognition begins, all types of events are delayed until gesture recognition fails.

The default value of this property is false.

## See Also

### Delaying Events

var delaysSecondaryMouseButtonEvents: Bool

A Boolean value that indicates whether secondary mouse button events are delivered only after gesture recognition fails.

var delaysOtherMouseButtonEvents: Bool

A Boolean value that indicates whether other mouse button events are delivered only after gesture recognition fails.

var delaysKeyEvents: Bool

A Boolean value that indicates whether key events are delivered only after gesture recognition fails.

var delaysMagnificationEvents: Bool

A Boolean value that indicates whether magnification events are delivered only after gesture recognition fails.

var delaysRotationEvents: Bool

A Boolean value that indicates whether rotation events are delivered only after gesture recognition fails.

