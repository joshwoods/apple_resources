

- Accessibility
- AXBrailleMap
-  height(at:) 

Instance Method

# height(at:)

Retrieves the height of an individual pin on the braille display.

iOS 15.2+iPadOS 15.2+Mac Catalyst 15.2+macOS 12.1+tvOS 15.2+visionOS 1.0+watchOS 8.2+

``` source
func height(at point: CGPoint) -> Float
```

## Parameters 

`point`  

The location of the pin to retrieve the height for. The bottom-left of the display is at `{ 0,0 }`, and the top-right of the display is at `{ dimensions.width - 1, dimensions.height - 1}`.

## Return Value

A floating-point number between `0.0` and `1.0` that specifies the height of the pin. A value of `0.0` indicates that the pin is completely lowered, and a value of `1.0` indicates that the pin is completely raised.

## See Also

### Accessing dots

func setHeight(Float, at: CGPoint)

Sets the height of an individual pin on the braille display.

subscript(CGPoint) -> Float

Accesses the height of an individual pin on the braille display.

