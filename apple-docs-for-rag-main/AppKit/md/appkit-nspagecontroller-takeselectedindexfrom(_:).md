

- AppKit
- NSPageController
-  takeSelectedIndexFrom(\_:) 

Instance Method

# takeSelectedIndexFrom(\_:)

Navigates to the selected index, which is taken from the sender.

macOS 10.8+

``` source
@IBAction @MainActor
func takeSelectedIndexFrom(_ sender: Any?)
```

## Parameters 

`sender`  

The control that invoked the action.

## Discussion

When invoked, this method causes the page controller’s view to display the object specified by the value taken from the `sender` control.

This method is animated and invokes the delegate’s pageControllerWillStartLiveTransition(_:) and pageControllerDidEndLiveTransition(_:) methods.

## See Also

### Related Documentation

func navigateForward(to: Any)

Navigates to the specific object.

### Page Controller Navigation

func navigateBack(Any?)

Navigates backwards in the page controller’s arranged objects array.

func navigateForward(Any?)

Navigates to the next object in the page controller’s arranged objects array, if appropriate.

