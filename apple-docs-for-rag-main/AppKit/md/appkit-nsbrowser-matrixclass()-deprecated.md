

- AppKit
- NSBrowser
-  matrixClass() Deprecated

Instance Method

# matrixClass()

Returns the matrix class used in the browser’s columns.

macOS 10.0–10.10Deprecated

``` source
@MainActor
func matrixClass() -> AnyClass
```

Deprecated

Use the item-based `NSBrowser` instead.

## Return Value

The class of `NSMatrix` used in the browser’s columns.

## See Also

### Deprecated

func column(of: NSMatrix) -> Int

Returns the column number in which the given matrix is located.

Deprecated

func matrix(inColumn: Int) -> NSMatrix?

Returns the matrix located in the specified column.

Deprecated

func setMatrixClass(AnyClass)

Sets the matrix class to be used in the browser’s columns.

Deprecated

