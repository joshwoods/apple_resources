

- Metal
- MTLIOCommandBuffer
-  addBarrier() 

Instance Method

# addBarrier()

Encodes a barrier into the command buffer.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
func addBarrier()
```

**Required**

## Discussion

The method encodes a barrier that starts any subsequent commands only after all the previously encoded commands have completed.

