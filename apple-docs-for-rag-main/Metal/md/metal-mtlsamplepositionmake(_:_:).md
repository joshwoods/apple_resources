

- Metal
-  MTLSamplePositionMake(\_:\_:) 

Function

# MTLSamplePositionMake(\_:\_:)

Returns a new sample position on a subpixel grid.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.13+tvOS 11.0+visionOS 1.0+

``` source
func MTLSamplePositionMake(
    _ x: Float,
    _ y: Float
) -> MTLSamplePosition
```

## Parameters 

`x`  

The x coordinate.

`y`  

The y coordinate.

## Return Value

The new sample position.

## See Also

### Using Programmable Sample Positions

func setSamplePositions([MTLSamplePosition])

Sets the programmable sample positions for a render pass.

func getSamplePositions() -> [MTLSamplePosition]

Returns the programmable sample positions set for a render pass.

