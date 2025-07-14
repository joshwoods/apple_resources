

- AppKit
- NSPageController
-  transitionStyle 

Instance Property

# transitionStyle

The transition style the page controller uses when changing pages.

macOS 10.8+

``` source
@MainActor
var transitionStyle: NSPageController.TransitionStyle { get set }
```

## Discussion

The possible values for the transition style are discussed in NSPageController.TransitionStyle.

The default value is NSPageController.TransitionStyle.stackHistory.

