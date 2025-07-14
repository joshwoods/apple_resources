

- Metal Performance Shaders Graph
- MPSGraph
-  coordinate(alongAxis:withShape:name:) 

Instance Method

# coordinate(alongAxis:withShape:name:)

Creates a get-coordindate operation and returns the result tensor.

iOS 15.4+iPadOS 15.4+Mac Catalyst 15.4+macOS 12.3+tvOS 15.4+visionOS 1.0+

``` source
func coordinate(
    alongAxis axis: Int,
    withShape shape: [NSNumber],
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`axis`  

The coordinate axis an element’s value is set to. Negative values wrap around.

`shape`  

The shape of the result tensor.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

## Discussion

Creates a tensor of specified shape with value at index `[i_0, i_1, ... , i_N] = i_axis` For example,

```
coordinateAlongAxis(0, withShape=[5]) = [0, 1, 2, 3, 4] 
coordinateAlongAxis(0, withShape=[3,2]) = [[0, 0],
                                           [1, 1],
                                           [2, 2]]
```

