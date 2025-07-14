

- AppKit
- NSColorWell
-  activate(\_:) 

Instance Method

# activate(\_:)

Activates the color well, displays the color panel, and synchronizes the two UI elements.

macOS

``` source
@MainActor
func activate(_ exclusive: Bool)
```

## Parameters 

`exclusive`  

true to deactivate any other color wells; false to keep them active. If a color panel is active with `exclusive` set to true and another is subsequently activated with `exclusive` set to false, the exclusive setting of the first panel is ignored.

## Discussion

When you call this method, the color well displays the standard color panel and sets the panel’s current color to the value in the color well. When someone changes the color in the color panel, the color well updates its selected color to match. If the color well’s isBordered property is true, the color well highlights that border while it’s active.

## See Also

### Activating and Deactivating Color Wells

var isActive: Bool

A Boolean value that indicates whether the color well is currently active.

func deactivate()

Deactivates the color well.

