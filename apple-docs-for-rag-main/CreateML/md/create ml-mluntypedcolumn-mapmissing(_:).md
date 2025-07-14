

- Create ML
- MLUntypedColumn
-  mapMissing(\_:) 

Instance Method

# mapMissing(\_:)

Creates a new column of typed values by applying the given thread-safe transform to every element of this untyped column, including missing elements.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func mapMissing(_ lazyTransform: @escaping (MLDataValue) -> T?) -> MLDataColumn where T : MLDataValueConvertible
```

## Parameters 

`lazyTransform`  

A thread-safe element transformation function. The implementation of the transform you provide should accept an element of the column and return a transformed value of a type that conforms to MLDataValueConvertible. If the transform returns `nil` for a given element, the corresponding element in the new column will have a missing value.

## Return Value

A new `MLDataColumn` column.

## See Also

### Transforming elements to generate a data column

func map&lt;T>((MLDataValue) -> T) -> MLDataColumn&lt;T>

Creates a new column of typed values by applying the given thread-safe transform to every non-missing element of this untyped column.

func map&lt;T>((MLDataValue) -> T?) -> MLDataColumn&lt;T>

Creates a new column of typed values, potentially with missing values, by applying the given thread-safe transform to every non-missing element of this untyped column.

