

- AppKit
- NSScrubber
- NSScrubber.Mode
-  NSScrubber.Mode.free 

Case

# NSScrubber.Mode.free

A scrolling mode in which the scrubber scrolls as the user swipes horizontally across the scrubber.

macOS 10.12.2+

``` source
case free
```

## Discussion

When a user swipes horizontally across the scrubber, the scrubber scrolls. To select an item, the user must tap or press it without moving their finger horizontally.

Free-mode interaction changes depending on the value the scrubber’s isContinuous property. For details on how to choose the correct mode for your app, see Choose a scrubber touch-interaction model.

## See Also

### Constants

case fixed

A scrolling mode in which scrubber items remain fixed in place, and the item under the user’s finger is highlighted.

