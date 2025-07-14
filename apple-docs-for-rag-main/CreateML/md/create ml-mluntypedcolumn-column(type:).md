

- Create ML
- MLUntypedColumn
-  column(type:) 

Instance Method

# column(type:)

Clones the column to a data column of the given type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func column(type: T.Type) -> MLDataColumn? where T : MLDataValueConvertible
```

## Parameters 

`type`  

A metatype used to create a new data column of that type.

## Return Value

A new data column if the underlying type of the column is the same as `type`; otherwise `nil`.

## Discussion

Use this method to create a typed copy of the column. For example, to create a data column of integers from an untyped column of integers, use column(type:) with Int`.self` as the argument for the `type` parameter.

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

var multiArrays: MLDataColumn&lt;MLDataValue.MultiArrayType>?

A cloned data column of machine learning multi-arrays.

