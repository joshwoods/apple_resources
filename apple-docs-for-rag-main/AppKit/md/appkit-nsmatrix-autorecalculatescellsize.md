

- AppKit
- NSMatrix
-  autorecalculatesCellSize 

Instance Property

# autorecalculatesCellSize

A Boolean that indicates whether the matrix auto-recalculates its cell size.

macOS 10.8+

``` source
@MainActor
var autorecalculatesCellSize: Bool { get set }
```

## Discussion

When the value of this property is true, auto-recalculation occurs. The matrix will adjust its cellSize to accommodate its largest cell. Changing the `cellSize` does not directly affect the frame of the matrix; however it does affect the intrinsic content size, which may cause the receiver to resize under Auto Layout. When using Auto Layout, you typically want this to be set to true.

The default value of this property is false.

