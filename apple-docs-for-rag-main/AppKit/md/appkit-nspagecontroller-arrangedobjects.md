

- AppKit
- NSPageController
-  arrangedObjects 

Instance Property

# arrangedObjects

An array containing the objects displayed in the page controller’s view.

macOS 10.8+

``` source
@MainActor
var arrangedObjects: [Any] { get set }
```

## Discussion

The delegate will be asked for snapshots as they are needed. Alternatively, you may never directly set this array and use the -navigateForward(to:) method to create a history as the user navigates.

This property is key-value observing compliant.

## See Also

### Page Controller Items

func navigateForward(to: Any)

Navigates to the specific object.

var selectedIndex: Int

The currently selected object in the arranged objects array.

