

- Create ML
- MLDataColumn
-  map(\_:) 

Instance Method

# map(\_:)

Creates a new column by applying the given thread-safe transform to every non-missing element of this column.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func map(_ lazyTransform: @escaping (Element) -> T) -> MLDataColumn where T : MLDataValueConvertible
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`lazyTransform`  

A thread-safe element transformation function. The implementation of the transform you provide should accept an `Element` of the column and return a transformed value of a type that conforms to MLDataValueConvertible.

## Return Value

A new column typed to the return type of `lazyTransform`.

## See Also

### Transforming elements to generate a column

func map&lt;T>((Element) -> T?) -> MLDataColumn&lt;T>

Creates a new column, potentially with missing values, by applying the given thread-safe transform to every non-missing element of this column.

func mapMissing&lt;T>((Element?) -> T?) -> MLDataColumn&lt;T>

Creates a new column, potentially with missing elements, by applying the given thread-safe transform to every element of the column, including missing elements.

