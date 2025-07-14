

- AppKit
- NSPageController
-  navigateForward(\_:) 

Instance Method

# navigateForward(\_:)

Navigates to the next object in the page controller’s arranged objects array, if appropriate.

macOS 10.8+

``` source
@IBAction @MainActor
func navigateForward(_ sender: Any?)
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

func navigateBack(Any?)

Navigates backwards in the page controller’s arranged objects array.

func takeSelectedIndexFrom(Any?)

Navigates to the selected index, which is taken from the sender.

