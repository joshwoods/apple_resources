

- Core Graphics
- CGWindowBackingType
-  CGWindowBackingType.backingStoreBuffered 

Case

# CGWindowBackingType.backingStoreBuffered

Mac CatalystmacOS

``` source
case backingStoreBuffered
```

## Discussion

The window draws into a display buffer and then flushes that buffer to the screen.

You should typically use this mode. It supports hardware acceleration, Quartz drawing, and takes advantage of the GPU when possible. It also supports alpha channel drawing, opacity controls, using the compositor.

## See Also

### Constants

case backingStoreNonretained

case backingStoreRetained

