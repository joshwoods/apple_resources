

- AppKit
- NSWindow
-  setIsMiniaturized(\_:) 

Instance Method

# setIsMiniaturized(\_:)

Sets the window’s miniaturized state to the value you specify.

macOS

``` source
@MainActor
func setIsMiniaturized(_ flag: Bool)
```

## Discussion

Depending on the current miniaturized state and the value of `flag`, the window may minimize to the Dock or expand from the Dock.

## See Also

### Setting Scripting Attributes

func setIsVisible(Bool)

Sets the window’s visible state to the value you specify.

func setIsZoomed(Bool)

Sets the window’s zoomed state to the value you specify.

