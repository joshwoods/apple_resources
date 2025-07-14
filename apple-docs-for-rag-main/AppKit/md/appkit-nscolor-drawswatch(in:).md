

- AppKit
- NSColor
-  drawSwatch(in:) 

Instance Method

# drawSwatch(in:)

Draws the current color in the specified rectangle.

macOS

``` source
func drawSwatch(in rect: NSRect)
```

## Parameters 

`rect`  

The rectangle in which to draw the color.

## Discussion

Subclasses adorn the rectangle in some manner to indicate the type of color. This method is invoked by color wells, swatches, and other user interface objects that need to display colors.

## See Also

### Drawing with Colors

func set()

Sets the color of subsequent drawing to the color that the color object represents.

func setFill()

Sets the fill color of subsequent drawing to the color object’s color.

func setStroke()

Sets the stroke color of subsequent drawing to the color object’s color.

