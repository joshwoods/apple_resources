

- TabularData
-  ShapedData 

Structure

# ShapedData

A collection type that represents multidimensional data in a data frame element.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
struct ShapedData
```

## Topics

### Initializers

init(shape: [Int], strides: [Int], contents: [Element])

Creates a multidimensional shaped array from a one-dimensional array.

### Instance Properties

let contents: [Element]

A linear array that stores the elements of the multidimensional array.

let shape: [Int]

An integer array that stores the size of each dimension in the corresponding element.

let strides: [Int]

An integer array that stores the number of memory locations that span the length of each dimension in the corresponding element.

### Subscripts

subscript(Int...) -> Element

Retrieves an element using an index for each dimension.

### Default Implementations

Equatable Implementations

Hashable Implementations

## Relationships

### Conforms To

- Copyable
- Equatable
- Hashable
- Sendable

## See Also

### Creating a Data Frame from Turi Create Types

init(contentsOfSFrameDirectory: URL, columns: [String]?, rows: Range&lt;Int>?) throws

Creates a data frame from a Turi Create scalable data frame.

