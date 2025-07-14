

- AppKit
- NSScrubberDelegate
-  scrubber(\_:didChangeVisibleRange:) 

Instance Method

# scrubber(\_:didChangeVisibleRange:)

Tells the delegate that the range of items currently visible in the scrubber has changed.

macOS 10.12.2+

``` source
@MainActor
optional func scrubber(
    _ scrubber: NSScrubber,
    didChangeVisibleRange visibleRange: NSRange
)
```

## Parameters 

`scrubber`  

The scrubber object that is notifying you of the change in the range of items that are currently visible.

`visibleRange`  

The range of items that are now visible in the scrubber.

