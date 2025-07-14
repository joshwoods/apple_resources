

- MetalFX
- MTLFXTemporalScaler
-  reset 

Instance Property

# reset

A Boolean that indicates whether the temporal scaler discards historical data from previous frames.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
var reset: Bool { get set }
```

**Required**

## Discussion

Set to true when the next frame your app encodes has no relevance to the previous frames, such as when changing scenes or perspectives.

## See Also

### Encoding a temporal scaling effect

func encode(commandBuffer: any MTLCommandBuffer)

Adds the temporal scaling command to a render pass’s command buffer.

**Required**

