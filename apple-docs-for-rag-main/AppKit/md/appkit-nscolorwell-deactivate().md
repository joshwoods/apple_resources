

- AppKit
- NSColorWell
-  deactivate() 

Instance Method

# deactivate()

Deactivates the color well.

macOS

``` source
@MainActor
func deactivate()
```

## Discussion

This method detaches the color well from the system color panel. Future selections in the color panel don’t update the color well’s current color.

## See Also

### Activating and Deactivating Color Wells

func activate(Bool)

Activates the color well, displays the color panel, and synchronizes the two UI elements.

var isActive: Bool

A Boolean value that indicates whether the color well is currently active.

