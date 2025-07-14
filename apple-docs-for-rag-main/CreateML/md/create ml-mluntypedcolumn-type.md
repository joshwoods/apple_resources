

- Create ML
- MLUntypedColumn
-  type 

Instance Property

# type

The underlying type of the column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
var type: MLDataValue.ValueType { get }
```

## Discussion

Use this to determine the underlying type of the column. Then use a corresponding property or method to create an MLDataColumn of the untyped column. For example, if type is equal to MLDataValue.ValueType.double, then use the MLUntypedColumn doubles property.

## See Also

### Exposing the underlying type to generate a data column

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

func column&lt;T>(type: T.Type) -> MLDataColumn&lt;T>?

Clones the column to a data column of the given type.

