

- UIKit
- UIInterfaceOrientation
-  isPortrait 

Instance Property

# isPortrait

A Boolean value that indicates whether the user interface is currently presented in a portrait orientation.

iOSiPadOSMac CatalystvisionOS

``` source
var isPortrait: Bool { get }
```

## Discussion

The interface orientation can be different than the device orientation. You typically call this function in your view controller code to check the current orientation.

## See Also

### Interface orientation

var isLandscape: Bool

A Boolean value that indicates whether the user interface is currently presented in a landscape orientation.

