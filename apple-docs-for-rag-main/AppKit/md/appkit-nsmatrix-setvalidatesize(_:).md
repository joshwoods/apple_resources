

- AppKit
- NSMatrix
-  setValidateSize(\_:) 

Instance Method

# setValidateSize(\_:)

Specifies whether the receiver’s size information is validated.

macOS

``` source
@MainActor
func setValidateSize(_ flag: Bool)
```

## Parameters 

`flag`  

true to assume that the size information in the receiver is correct. If `flag` is false, the NSControl method calcSize() will be invoked before any further drawing is done.

## See Also

### Resizing the Matrix and Its Cells

var autosizesCells: Bool

A Boolean that indicates whether the cell sizes change when the receiver is resized.

func sizeToCells()

Changes the width and the height of the receiver’s frame so it exactly contains the cells.

