

- Metal
- MTLIndirectCommandBuffer
-  reset(\_:) 

Instance Method

# reset(\_:)

Resets a range of commands to their default state.

iOS 12.0+iPadOS 12.0+Mac CatalystmacOS 10.14+tvOS 12.0+visionOS

``` source
func reset(_ range: Range)
```

## Parameters 

`range`  

The range of commands to reset. The range must fit inside the indirect command buffer’s extents.

