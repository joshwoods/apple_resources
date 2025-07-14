

- TabularData
- DiscontiguousColumnSlice
-  name 

Instance Property

# name

The name of the slice’s parent column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var name: String { get set }
```

## See Also

### Inspecting a Column Slice

var count: Int

The number of elements in the column slice.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

func argmin() -> Int?

Returns the index of the element with the lowest value, ignoring missing elements.

func argmax() -> Int?

Returns the index of the element with the highest value, ignoring missing elements.

func isNil(at: Int) -> Bool

Returns a Boolean that indicates whether the element at the index is missing.

