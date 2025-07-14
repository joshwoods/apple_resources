

- AppKit
- NSScrubber
- NSScrubber.Mode
-  NSScrubber.Mode.fixed 

Case

# NSScrubber.Mode.fixed

A scrolling mode in which scrubber items remain fixed in place, and the item under the user’s finger is highlighted.

macOS 10.12.2+

``` source
case fixed
```

## Discussion

When a user swipes horizontally across the scrubber, the scrubber items remain fixed in place and the item under the user’s finger highlights. At the conclusion of the touch interaction, the last-highlighted item is selected.

For details on how to choose the correct mode for your app, see Choose a scrubber touch-interaction model.

## See Also

### Constants

case free

A scrolling mode in which the scrubber scrolls as the user swipes horizontally across the scrubber.

