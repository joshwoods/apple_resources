

- AppKit
- NSBrowser
-  matrix(inColumn:) Deprecated

Instance Method

# matrix(inColumn:)

Returns the matrix located in the specified column.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func matrix(inColumn column: Int) -> NSMatrix?
```

Deprecated

Use the item-based `NSBrowser` instead.

## Parameters 

`column`  

The column index of the matrix to obtain.

## Return Value

The matrix located in the column.

## See Also

### Deprecated

func column(of: NSMatrix) -> Int

Returns the column number in which the given matrix is located.

Deprecated

func matrixClass() -> AnyClass

Returns the matrix class used in the browser’s columns.

Deprecated

func setMatrixClass(AnyClass)

Sets the matrix class to be used in the browser’s columns.

Deprecated

