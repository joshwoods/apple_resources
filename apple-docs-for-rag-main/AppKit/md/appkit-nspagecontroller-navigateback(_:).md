

- AppKit
- NSPageController
-  navigateBack(\_:) 

Instance Method

# navigateBack(\_:)

Navigates backwards in the page controller’s arranged objects array.

macOS 10.8+

``` source
@IBAction @MainActor
func navigateBack(_ sender: Any?)
```

## Parameters 

`sender`  

The sender.

## Discussion

This method is typically invoked in response to a user interacting with a control, the `sender`.

This method is animated and invokes the delegate’s pageControllerWillStartLiveTransition(_:) and pageControllerDidEndLiveTransition(_:) methods.

## See Also

### Related Documentation

func navigateForward(to: Any)

Navigates to the specific object.

### Page Controller Navigation

func navigateForward(Any?)

Navigates to the next object in the page controller’s arranged objects array, if appropriate.

func takeSelectedIndexFrom(Any?)

Navigates to the selected index, which is taken from the sender.

