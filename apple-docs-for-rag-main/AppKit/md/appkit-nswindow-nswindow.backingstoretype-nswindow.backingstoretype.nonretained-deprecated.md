

- AppKit
- NSWindow
- NSWindow.BackingStoreType
-  NSWindow.BackingStoreType.nonretained Deprecated

Case

# NSWindow.BackingStoreType.nonretained

The window draws directly to the screen without using any buffer.

macOS 10.0–10.13Deprecated

``` source
case nonretained
```

## Discussion

You should not use this mode. It exists primarily for use in the original Classic Blue Box. It does not support Quartz drawing, alpha blending, or opacity. Moreover, it does not support hardware acceleration, and interferes with system-wide display acceleration. If you use this mode, your application must manage visibility region clipping itself, and manage repainting on visibility changes.

## See Also

### Constants

case retained

The window uses a buffer, but draws directly to the screen where possible and to the buffer for obscured portions.

Deprecated

case buffered

The window renders all drawing into a display buffer and then flushes it to the screen.

