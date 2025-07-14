

- Create ML
- MLUntypedColumn
-  ints 

Instance Property

# ints

A cloned data column of integers.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var ints: MLDataColumn? { get }
```

## Return Value

A new data column if the underlying type of the column is Int; otherwise `nil`.

## Discussion

This property is functionally equivalent to passing Int`.self` to column(type:). Typically you ensure type is equal to MLDataValue.ValueType.int before getting this property.

## See Also

### Exposing the underlying type to generate a data column

var type: MLDataValue.ValueType

The underlying type of the column.

var doubles: MLDataColumn&lt;Double>?

A cloned data column of doubles.

var strings: MLDataColumn&lt;String>?

A cloned data column of strings.

var sequences: MLDataColumn&lt;MLDataValue.SequenceType>?

A cloned data column of machine learning sequences.

var dictionaries: MLDataColumn&lt;MLDataValue.DictionaryType>?

A cloned data column of machine learning dictionaries.

var multiArrays: MLDataColumn&lt;MLDataValue.MultiArrayType>?

A cloned data column of machine learning multi-arrays.

func column&lt;T>(type: T.Type) -> MLDataColumn&lt;T>?

Clones the column to a data column of the given type.

