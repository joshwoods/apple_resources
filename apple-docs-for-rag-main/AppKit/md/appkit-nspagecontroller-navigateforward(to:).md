

- AppKit
- NSPageController
-  navigateForward(to:) 

Instance Method

# navigateForward(to:)

Navigates to the specific object.

macOS 10.8+

``` source
@MainActor
func navigateForward(to object: Any)
```

## Parameters 

`object`  

The object to display.

## Discussion

Clears the arrangedObjects array after the selected index, adds the argument to that array, and sets the selectedIndex to the object’s index.

## See Also

### Related Documentation

func takeSelectedIndexFrom(Any?)

Navigates to the selected index, which is taken from the sender.

func navigateBack(Any?)

Navigates backwards in the page controller’s arranged objects array.

func navigateForward(Any?)

Navigates to the next object in the page controller’s arranged objects array, if appropriate.

### Page Controller Items

var arrangedObjects: [Any]

An array containing the objects displayed in the page controller’s view.

var selectedIndex: Int

The currently selected object in the arranged objects array.

