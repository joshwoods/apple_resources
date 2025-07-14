

- Accelerate
-  BNNSGraphContextSetStreamingAdvanceCount(\_:\_:) 

Function

# BNNSGraphContextSetStreamingAdvanceCount(\_:\_:)

Sets streaming advancement amount for cases with dynamically shaped inputs.

iOS 18.4+iPadOS 18.4+Mac Catalyst 18.4+macOS 15.4+tvOS 18.4+visionOS 2.4+watchOS 11.4+

``` source
func BNNSGraphContextSetStreamingAdvanceCount(
    _ context: bnns_graph_context_t,
    _ advance_count: Int
) -> Int32
```

## Discussion

For models compiled with the `BNNSOption` attribute `StateMode=Streaming` enabled, where `slice_update` ops use an update parameter of dynamic shape, BNNS cannot unambigiously determine the streaming advancement size. Instead the user must use this function *prior* to calling `BNNSGraphContextExecute()` to set the advancement size for each frame.

The internal state pointer will then be advanced by `advance_count` elements in the streaming dimension prior to returning from `BNNSGraphContextExecute()`. The BNNS streaming APIs do not support models that require different advancement amounts for different states.

