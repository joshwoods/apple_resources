

- Metal Performance Shaders Graph
- MPSGraph
-  if(\_:then:else:name:) 

Instance Method

# if(\_:then:else:name:)

Adds an if-then-else operation to the graph.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
func `if`(
    _ predicateTensor: MPSGraphTensor,
    then thenBlock: @escaping MPSGraphIfThenElseBlock,
    else elseBlock: MPSGraphIfThenElseBlock?,
    name: String?
) -> [MPSGraphTensor]
```

## Parameters 

`predicateTensor`  

Tensor must have a single scalar value, used to decide between then/else branches

`thenBlock`  

If predicate is true operations in this block are executed

`elseBlock`  

If predicate is false operations in this block are executed

`name`  

Name of operation

## Return Value

Results If no error, the tensors returned by user. If not empty, user must define both then/else block, both should have same number of arguments and each corresponding argument should have same elementTypes.

