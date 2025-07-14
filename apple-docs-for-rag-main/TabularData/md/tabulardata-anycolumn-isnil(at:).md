

- TabularData
- AnyColumn
-  isNil(at:) 

Instance Method

# isNil(at:)

Returns a Boolean that indicates whether the element at the index is missing.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
func isNil(at index: Int) -> Bool
```

## Parameters 

`index`  

The location of an element in the column.

## See Also

### Inspecting a Type-Erased Column

var name: String

The name of the column.

var count: Int

The number of elements in the column.

var missingCount: Int

The number of missing elements in the column.

var wrappedElementType: any Any.Type

The underlying type of the column’s elements.

