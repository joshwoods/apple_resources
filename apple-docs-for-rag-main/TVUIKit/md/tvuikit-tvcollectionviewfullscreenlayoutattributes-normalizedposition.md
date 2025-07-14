

- TVUIKit
- TVCollectionViewFullScreenLayoutAttributes
-  normalizedPosition 

Instance Property

# normalizedPosition

A value that indicates the distance of the current cell from the collection view’s center cell.

tvOS 13.0+

``` source
@MainActor
var normalizedPosition: CGFloat { get set }
```

## Discussion

A negative value indicates that the cell is positioned to the left of the center cell in the collection view. A positive value indicates that the cell is positioned to the right of the center cell. A 0 value indicates the cell is in the neutral position, in the center of the collection view.

