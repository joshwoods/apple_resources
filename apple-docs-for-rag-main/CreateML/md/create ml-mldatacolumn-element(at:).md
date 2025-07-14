

- Create ML
- MLDataColumn
-  element(at:) 

Instance Method

# element(at:)

Accesses the element at the given index.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
func element(at index: Int) -> Element?
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`index`  

A row number of the column, beginning with `0`.

## Return Value

The `Element` at the given index; otherwise, `nil`.

## See Also

### Getting an element

subscript(Int) -> Element

Accesses the element at the given row.

