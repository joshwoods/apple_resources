

- AppKit
- NSPageController
-  selectedIndex 

Instance Property

# selectedIndex

The currently selected object in the arranged objects array.

macOS 10.8+

``` source
@MainActor
var selectedIndex: Int { get set }
```

## Discussion

To animate a transition to a new index, use the NSPageController class animator object.

This property is key-value observing compliant.

## See Also

### Page Controller Items

var arrangedObjects: [Any]

An array containing the objects displayed in the page controller’s view.

func navigateForward(to: Any)

Navigates to the specific object.

