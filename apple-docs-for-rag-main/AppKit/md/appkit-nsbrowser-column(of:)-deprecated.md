

- AppKit
- NSBrowser
-  column(of:) Deprecated

Instance Method

# column(of:)

Returns the column number in which the given matrix is located.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func column(of matrix: NSMatrix) -> Int
```

Deprecated

Use the item-based `NSBrowser` instead.

## Parameters 

`matrix`  

The matrix for which to return the column number.

## Return Value

The index of the column in which the specified matrix appears.

## See Also

### Deprecated

func matrix(inColumn: Int) -> NSMatrix?

Returns the matrix located in the specified column.

Deprecated

func matrixClass() -> AnyClass

Returns the matrix class used in the browser’s columns.

Deprecated

func setMatrixClass(AnyClass)

Sets the matrix class to be used in the browser’s columns.

Deprecated

