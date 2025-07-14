

- Create ML Components
- ClassificationDistribution
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a classification at an index.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
subscript(index: Int) -> Classification { get }
```

## Parameters 

`index`  

A valid index to a classification in the classification distribution.

## See Also

### Accessing by subscript

subscript(Range&lt;Int>) -> Slice&lt;ClassificationDistribution&lt;Label>>

Accesses a contiguous range of elements.

subscript(Label) -> Float?

Accesses a probability with label.

