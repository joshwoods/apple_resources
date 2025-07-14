

- Create ML
- MLUntypedColumn
-  map(to:) 

Instance Method

# map(to:)

Creates a new column of typed values by converting this untyped column to the given type.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func map(to type: T.Type) -> MLDataColumn where T : MLDataValueConvertible
```

## Parameters 

`type`  

A metatype used to create a new data column of that type.

## Return Value

A new data column if the column’s underlying type is convertible to given type; otherwise `nil`.

## Discussion

Use this method to convert the elements of the column to a data column of the given type via MLDataValueConvertible. Unlike column(type:), which doesn’t alter its elements, map(to:) converts the elements to the destination type. For example, you can use map(to:) to convert an untyped column of integers to a data column of strings.

