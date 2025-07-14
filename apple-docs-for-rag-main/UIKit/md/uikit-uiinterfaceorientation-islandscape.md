

- UIKit
- UIInterfaceOrientation
-  isLandscape 

Instance Property

# isLandscape

A Boolean value that indicates whether the user interface is currently presented in a landscape orientation.

iOSiPadOSMac CatalystvisionOS

``` source
var isLandscape: Bool { get }
```

## Discussion

The interface orientation can be different than the device orientation. You typically call this function in your view controller code to check the current orientation.

## See Also

### Interface orientation

var isPortrait: Bool

A Boolean value that indicates whether the user interface is currently presented in a portrait orientation.

