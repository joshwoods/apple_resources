

- Create ML Components
- ClassificationDistribution
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses a probability with label.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+watchOS 11.0+

``` source
subscript(label: Label) -> Float? { get }
```

## Parameters 

`label`  

A label in the classification set.

## See Also

### Accessing by subscript

subscript(Range&lt;Int>) -> Slice&lt;ClassificationDistribution&lt;Label>>

Accesses a contiguous range of elements.

subscript(Int) -> Classification&lt;Label>

Accesses a classification at an index.

