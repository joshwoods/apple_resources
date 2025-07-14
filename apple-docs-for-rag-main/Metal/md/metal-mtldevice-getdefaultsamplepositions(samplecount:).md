

- Metal
- MTLDevice
-  getDefaultSamplePositions(sampleCount:) 

Instance Method

# getDefaultSamplePositions(sampleCount:)

Returns the default sample locations based on the number of samples.

iOS 11.0+iPadOS 11.0+Mac CatalystmacOS 10.13+tvOS 11.0+visionOS

``` source
func getDefaultSamplePositions(sampleCount: Int) -> [MTLSamplePosition]
```

## Parameters 

`sampleCount`  

The number of points a GPU can sample from a texture. Ensure the GPU can support the `sampleCount` value by first calling the device’s supportsTextureSampleCount(_:) method.

## Return Value

An array of MTLSamplePosition instances.

## Discussion

The default sample positions are the same on all GPUs that support programmable sample positions (see areProgrammableSamplePositionsSupported).

Note

GPUs that don’t support programmable sample positions may have different default sample positions that you can’t retrieve.

The default sample position for GPUs that can sample one time is at the pixel’s center.

The default sample positions for GPUs that can sample two times have locations in the center of the pixel’s second quadrant and fourth quadrants.

The default sample positions for GPUs that can sample four times have one location in each of the pixel’s quadrants. Each location is at the center of one of that quadrant’s subquadrants.

The default sample positions for GPUs that can sample eight times have two locations in each of the pixel’s quadrants.

The table lists the indices and default locations for GPUs that support one, two, four, or eight sample positions.

| Sample count | Position indices | Subpixel coordinates |
|----|----|----|
| 1 | 0 | (0.5, 0.5) |
| 2 | 0  1 | (0.75, 0.75)  (0.25, 0.25) |
| 4 | 0  1  2  3 | (0.375, 0.125)  (0.875, 0.375)  (0.125, 0.625)  (0.625, 0.875) |
| 8 | 0  1  2  3  4  5  6  7 | (0.5625, 0.3125)  (0.4375, 0.6875)  (0.8125, 0.5625)  (0.3125, 0.1875)  (0.1875, 0.8125)  (0.0625, 0.4375)  (0.6875, 0.9375)  (0.9375, 0.0625) |

## See Also

### Creating Samplers

func supportsTextureSampleCount(Int) -> Bool

Returns a Boolean value that indicates whether the GPU can sample a texture with a specific number of sample points.

**Required**

func makeSamplerState(descriptor: MTLSamplerDescriptor) -> (any MTLSamplerState)?

Creates a sampler state instance.

**Required**

