

- UIKit
- UIColor
-  setStroke() 

Instance Method

# setStroke()

Sets the color of subsequent stroke operations to the color that the receiver represents.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+watchOS 2.0+

``` source
func setStroke()
```

## Discussion

If you subclass `UIColor`, you must implement this method in your subclass. Your custom implementation should modify the stroke color in the current graphics context by setting it to the color represented by the receiver.

## See Also

### Applying the color to the drawing environment

Customizing drawings

Create custom colors and patterns for drawing in your app.

func set()

Sets the color of subsequent stroke and fill operations to the color that the receiver represents.

func setFill()

Sets the color of subsequent fill operations to the color that the receiver represents.

