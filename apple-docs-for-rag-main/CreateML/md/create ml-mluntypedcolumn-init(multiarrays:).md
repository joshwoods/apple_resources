

- Create ML
- MLUntypedColumn
-  init(multiArrays:) 

Initializer

# init(multiArrays:)

Creates a MLUntypedColumn of type MLMultiArray from the specified MLUntypedColumn if the values of the given MLUntypedColumn are convertible to MLDataValue.MultiArrayType.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
init(multiArrays: MLUntypedColumn)
```

## Parameters 

`multiArrays`  

A MLUntypedColumn from which to create a MLUntypedColumn with type MLDataValue.DictionaryType

## Return Value

A MLUntypedColumn of type MultiArray from the specified MLUntypedColumn if the given MLUntypedColumn’s values are convertible to MLDataValue.MultiArrayType. Returns an invalid MLUntypedColumn if the elements in the given MLUntypedColumn are not convertible to MLDataValue.MultiArrayType.

## See Also

### Creating an untyped column by converting another column

init(ints: MLUntypedColumn)

Creates a new column of integers by converting the elements of another column.

init(doubles: MLUntypedColumn)

Creates a new column of doubles by converting the elements of another column.

init(strings: MLUntypedColumn)

Creates a new column of strings by converting the elements of another column.

init(sequences: MLUntypedColumn)

Creates a new column of machine learning sequences by converting the elements of another column.

init(dictionaries: MLUntypedColumn)

Creates a new column of machine learning dictionaries by converting the elements of another column.

