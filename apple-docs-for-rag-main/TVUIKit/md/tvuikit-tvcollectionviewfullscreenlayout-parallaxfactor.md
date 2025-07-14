

- TVUIKit
- TVCollectionViewFullScreenLayout
-  parallaxFactor 

Instance Property

# parallaxFactor

A value that specifies how slowly the background should move relative to the foreground.

tvOS 13.0+

``` source
@MainActor
var parallaxFactor: CGFloat { get set }
```

## Discussion

A large `parallaxFactor` value causes the background to move more slowly compared to the foreground. A small value makes the foreground and background move at a similar pace. The parallax effect becomes more apparent as the value of `parallaxFactor` increases.

The default value of this property is 0.8. The minimum value is 0.0.

## See Also

### Managing transitions

var isTransitioningToCenterIndexPath: Bool

A Boolean value that indicates whether the cell is changing index paths.

