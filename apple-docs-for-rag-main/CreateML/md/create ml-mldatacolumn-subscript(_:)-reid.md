

- Create ML
- MLDataColumn
-  subscript(\_:) 

Instance Subscript

# subscript(\_:)

Accesses the element at the given row.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 10.14+tvOS 16.0+visionOS 1.0+

``` source
subscript(index: Int) -> Element { get }
```

Available when `Element` conforms to `MLDataValueConvertible`.

## Parameters 

`index`  

A row number of the column, beginning with `0`.

## Return Value

The `Element` at the given index.

## See Also

### Getting an element

func element(at: Int) -> Element?

Accesses the element at the given index.

