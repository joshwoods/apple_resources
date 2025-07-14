

- Create ML
- MLUntypedColumn
-  multiArrays 

Instance Property

# multiArrays

A cloned data column of machine learning multi-arrays.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var multiArrays: MLDataColumn? { get }
```

## Return Value

A new data column if the underlying type of the column is MLDataValue.MultiArrayType; otherwise `nil`.

## Discussion

This property is functionally equivalent to passing MLDataValue.MultiArrayType `.self` to column(type:). Typically you ensure type is equal to MLDataValue.ValueType.multiArray before getting this property.

## See Also

### Exposing the underlying type to generate a data column

var type: MLDataValue.ValueType

The underlying type of the column.

var ints: MLDataColumn&lt;Int>?

A cloned data column of integers.

var doubles: MLDataColumn&lt;Double>?

A cloned data column of doubles.

var strings: MLDataColumn&lt;String>?

A cloned data column of strings.

var sequences: MLDataColumn&lt;MLDataValue.SequenceType>?

A cloned data column of machine learning sequences.

var dictionaries: MLDataColumn&lt;MLDataValue.DictionaryType>?

A cloned data column of machine learning dictionaries.

func column&lt;T>(type: T.Type) -> MLDataColumn&lt;T>?

Clones the column to a data column of the given type.

