

- MetalFX
- MTLFXTemporalScaler
-  encode(commandBuffer:) 

Instance Method

# encode(commandBuffer:)

Adds the temporal scaling command to a render pass’s command buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+

``` source
func encode(commandBuffer: any MTLCommandBuffer)
```

**Required**

## Parameters 

`commandBuffer`  

The destination command buffer for a render pass.

## See Also

### Encoding a temporal scaling effect

var reset: Bool

A Boolean that indicates whether the temporal scaler discards historical data from previous frames.

**Required**

