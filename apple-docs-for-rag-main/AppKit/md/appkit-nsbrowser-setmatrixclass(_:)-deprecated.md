

- AppKit
- NSBrowser
-  setMatrixClass(\_:) Deprecated

Instance Method

# setMatrixClass(\_:)

Sets the matrix class to be used in the browser’s columns.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func setMatrixClass(_ factoryId: AnyClass)
```

Deprecated

Use the item-based `NSBrowser` instead.

## Parameters 

`factoryId`  

The matrix class (`NSMatrix` or an `NSMatrix` subclass) used in the browser’s columns.

## See Also

### Deprecated

func column(of: NSMatrix) -> Int

Returns the column number in which the given matrix is located.

Deprecated

func matrix(inColumn: Int) -> NSMatrix?

Returns the matrix located in the specified column.

Deprecated

func matrixClass() -> AnyClass

Returns the matrix class used in the browser’s columns.

Deprecated

