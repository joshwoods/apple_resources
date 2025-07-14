

- WatchKit
- WKApplication
-  rootInterfaceController 

Instance Property

# rootInterfaceController

The app’s root interface controller.

watchOS 7.0+

``` source
@MainActor
var rootInterfaceController: WKInterfaceController? { get }
```

## Discussion

The root interface controller is located in the app’s main storyboard and has the Main Entry Point object associated with it. WatchKit displays the root interface controller at launch time, although the app can present a different interface controller before the launch sequence finishes.

## See Also

### Getting the interface controller

var visibleInterfaceController: WKInterfaceController?

Returns the last visible interface controller.

