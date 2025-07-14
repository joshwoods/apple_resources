

- TVUIKit
- TVCollectionViewFullScreenCell
-  normalizedPosition 

Instance Property

# normalizedPosition

The value that determines the current cell’s relative position on the screen.

tvOS 13.0+

``` source
@MainActor
var normalizedPosition: CGFloat { get }
```

## Discussion

A value of 0 indicates that the cell is positioned at the center of the collection view. A negative value indicates that the cell is positioned to the left of the center. A positive value indicates that the cell is positioned to the right of the center.

