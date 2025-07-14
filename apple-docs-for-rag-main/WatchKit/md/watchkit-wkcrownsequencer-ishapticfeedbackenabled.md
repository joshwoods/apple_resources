

- WatchKit
- WKCrownSequencer
-  isHapticFeedbackEnabled 

Instance Property

# isHapticFeedbackEnabled

A Boolean value that determines whether the crown sequencer’s haptic feedback is enabled.

watchOS 5.0+

``` source
var isHapticFeedbackEnabled: Bool { get set }
```

## Discussion

By default, this property is set to true. In Apple Watch Series 4 and later, the watch provides linear haptic feedback as the user rotates the digital crown. Set this property to false to disable the haptic feedback while the crown sequencer has the focus. For example, you can use this property to disable haptic feedback if the feedback does not match the screen’s animation.

## See Also

### Related Documentation

var isTableScrollingHapticFeedbackEnabled: Bool

A Boolean value that determines whether haptic feedback coordinates with the appearance of new rows as the user scrolls through a table.

