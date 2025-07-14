

- Create ML Components
- ClassificationDistribution
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a contiguous range of elements.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
subscript(bounds: Range) -> Slice> { get }
```

## Parameters 

`bounds`  

A range of valid indices in the classification distribution.

## See Also

### Accessing by subscript

subscript(Int) -> Classification&lt;Label>

Accesses a classification at an index.

subscript(Label) -> Float?

Accesses a probability with label.

