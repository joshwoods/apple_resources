

- AppKit
- NSWindow
- NSWindow.BackingStoreType
-  NSWindow.BackingStoreType.buffered 

Case

# NSWindow.BackingStoreType.buffered

The window renders all drawing into a display buffer and then flushes it to the screen.

macOS

``` source
case buffered
```

## Discussion

You should use this mode. It supports hardware acceleration, Quartz drawing, and takes advantage of the GPU when possible. It also supports alpha channel drawing, opacity controls, using the compositor.

## See Also

### Constants

case retained

The window uses a buffer, but draws directly to the screen where possible and to the buffer for obscured portions.

Deprecated

case nonretained

The window draws directly to the screen without using any buffer.

Deprecated

