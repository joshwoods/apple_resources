

- UIKit
- UICollectionViewLayout
-  developmentLayoutDirection 

Instance Property

# developmentLayoutDirection

The direction of the language you used when designing your custom layout.

iOSiPadOSMac CatalysttvOSvisionOS

``` source
@MainActor
var developmentLayoutDirection: UIUserInterfaceLayoutDirection { get }
```

## Discussion

The default value of this property is the layout direction used by the language associated with the main bundle’s development region. Subclasses may override this property and return a different value.

## See Also

### Supporting right-to-left layouts

var flipsHorizontallyInOppositeLayoutDirection: Bool

A Boolean value that indicates whether the horizontal coordinate system is automatically flipped at appropriate times.

