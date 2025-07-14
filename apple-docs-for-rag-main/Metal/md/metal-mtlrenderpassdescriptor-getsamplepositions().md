

- Metal
- MTLRenderPassDescriptor
-  getSamplePositions() 

Instance Method

# getSamplePositions()

Returns the programmable sample positions set for a render pass.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOS

``` source
func getSamplePositions() -> [MTLSamplePosition]
```

## Return Value

An array of programmable sample positions.

## See Also

### Using Programmable Sample Positions

func MTLSamplePositionMake(Float, Float) -> MTLSamplePosition

Returns a new sample position on a subpixel grid.

func setSamplePositions([MTLSamplePosition])

Sets the programmable sample positions for a render pass.

