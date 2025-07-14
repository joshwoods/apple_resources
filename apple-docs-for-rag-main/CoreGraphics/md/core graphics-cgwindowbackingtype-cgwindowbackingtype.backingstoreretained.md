

- Core Graphics
- CGWindowBackingType
-  CGWindowBackingType.backingStoreRetained 

Case

# CGWindowBackingType.backingStoreRetained

Mac CatalystmacOS

``` source
case backingStoreRetained
```

## Discussion

The window uses a buffer, but draws directly to the screen where possible and to the buffer for obscured portions.

You should typically not use this mode. It combines the limitations of CGWindowBackingType.backingStoreNonretained with the memory use of CGWindowBackingType.backingStoreBuffered. The original NeXTSTEP implementation was an interesting compromise that worked well with fast memory mapped framebuffers on the CPU bus—something that hasn’t been in general use since around 1994. These tend to have performance problems.

In macOS 10.5 and later, requests for retained windows will result in the window system creating a buffered window, as that better matches actual use

## See Also

### Constants

case backingStoreBuffered

case backingStoreNonretained

