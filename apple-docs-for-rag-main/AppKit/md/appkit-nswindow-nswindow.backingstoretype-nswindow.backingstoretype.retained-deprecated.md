

- AppKit
- NSWindow
- NSWindow.BackingStoreType
-  NSWindow.BackingStoreType.retained Deprecated

Case

# NSWindow.BackingStoreType.retained

The window uses a buffer, but draws directly to the screen where possible and to the buffer for obscured portions.

macOS 10.0–10.13Deprecated

``` source
case retained
```

## Discussion

You should not use this mode. It combines the limitations of `NSBackingStoreNonretained` with the memory use of `NSBackingStoreBuffered`. The original NeXTSTEP implementation was an interesting compromise that worked well with fast memory mapped framebuffers on the CPU bus—something that hasn’t been in general use since around 1994. These tend to have performance problems.

In macOS 10.5 and later, requests for retained windows will result in the window system creating a buffered window, as that better matches actual use.

## See Also

### Constants

case nonretained

The window draws directly to the screen without using any buffer.

Deprecated

case buffered

The window renders all drawing into a display buffer and then flushes it to the screen.

