

- TabularData
- AnyColumn
-  prototype 

Instance Property

# prototype

A prototype that creates type-erased columns with the same underlying type as the column slice.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
var prototype: any AnyColumnPrototype { get }
```

## Discussion

Use a type-erased column prototype to create new columns of the same type as the slice’s parent column without explicitly knowing what type it is, by calling the `prototype` property’s makeColumn(capacity:) method.

```
```

