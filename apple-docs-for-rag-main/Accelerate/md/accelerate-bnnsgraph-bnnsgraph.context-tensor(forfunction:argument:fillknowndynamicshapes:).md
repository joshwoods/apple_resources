

- Accelerate
- BNNSGraph
- BNNSGraph.Context
-  tensor(forFunction:argument:fillKnownDynamicShapes:) 

Instance Method

# tensor(forFunction:argument:fillKnownDynamicShapes:)

Returns an unallocated tensor for a given function argument.

iOS 18.0+iPadOS 18.0+Mac CatalystmacOS 15.0+tvOS 18.0+visionOSwatchOS 11.0+

``` source
func tensor(
    forFunction function: String? = nil,
    argument: String,
    fillKnownDynamicShapes: Bool
) -> BNNSTensor?
```

## Parameters 

`function`  

The function. Specify as `nil` if the graph only contains one function.

`argument`  

The name of the input or output argument.

`fillKnownDynamicShapes`  

A Boolean value that specifies whether the function should replace any dynamic shapes for the next execution of the context. BNNS derives these shapes either from the default shapes in the source model, or from preceding calls to setDynamicShapes(_:forFunction:) or setBatchSize(_:forFunction:). If BNNS is unable to derive the shapes, the function sets the dimensions to `-1`.

## See Also

### Related Documentation

func BNNSGraphContextGetTensor(bnns_graph_context_t, UnsafePointer&lt;CChar>?, UnsafePointer&lt;CChar>, Bool, UnsafeMutablePointer&lt;BNNSTensor>) -> Int32

Sets the properties of a tensor for the specified function argument.

