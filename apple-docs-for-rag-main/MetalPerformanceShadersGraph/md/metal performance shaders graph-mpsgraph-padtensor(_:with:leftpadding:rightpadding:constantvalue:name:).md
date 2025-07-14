

- Metal Performance Shaders Graph
- MPSGraph
-  padTensor(\_:with:leftPadding:rightPadding:constantValue:name:) 

Instance Method

# padTensor(\_:with:leftPadding:rightPadding:constantValue:name:)

Creates a padding operation and returns the result tensor.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+

``` source
func padTensor(
    _ tensor: MPSGraphTensor,
    with paddingMode: MPSGraphPaddingMode,
    leftPadding: [NSNumber],
    rightPadding: [NSNumber],
    constantValue: Double,
    name: String?
) -> MPSGraphTensor
```

## Parameters 

`tensor`  

The input tensor.

`paddingMode`  

The parameter that defines the padding mode.

`leftPadding`  

The parameter that defines how much padding the operation applies to the input tensor before each dimension - must be of size `rank(tensor)`.

`rightPadding`  

The parameter that defines how much padding the operation applies to the input tensor after each dimension - must be of size `rank(tensor)`.

`constantValue`  

The constant value the operation uses when `paddingMode = MPSGraphPaddingModeConstant`.

`name`  

The name for the operation.

## Return Value

A valid MPSGraphTensor object.

