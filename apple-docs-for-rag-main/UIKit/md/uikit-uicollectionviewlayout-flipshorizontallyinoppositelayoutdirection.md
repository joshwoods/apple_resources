

- UIKit
- UICollectionViewLayout
-  flipsHorizontallyInOppositeLayoutDirection 

Instance Property

# flipsHorizontallyInOppositeLayoutDirection

A Boolean value that indicates whether the horizontal coordinate system is automatically flipped at appropriate times.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var flipsHorizontallyInOppositeLayoutDirection: Bool { get }
```

## Discussion

The language you use during development naturally affects the decisions you make when configuring your layout object. When you develop using a left-to-right language, your layout information automatically matches the collection view’s natural coordinate system. However, when the user’s language has a right-to-left orientation, the layout information you provide is still based on the collection view’s natural coordinate system. This discrepancy can cause layout issues for languages using the opposite orientation. When this property is set to true, the collection view automatically flips the orientation of its horizontal coordinate system to match the leading edge of the current language. (The developmentLayoutDirection property specifies the layout direction used to design the layout.) Flipping the horizontal coordinate system effectively flips your existing layout information, which should result in a better looking layout.

The default value of this property is false.

## See Also

### Supporting right-to-left layouts

var developmentLayoutDirection: UIUserInterfaceLayoutDirection

The direction of the language you used when designing your custom layout.

