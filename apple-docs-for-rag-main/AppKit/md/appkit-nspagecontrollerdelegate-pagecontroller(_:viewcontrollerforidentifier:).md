

- AppKit
- NSPageControllerDelegate
-  pageController(\_:viewControllerForIdentifier:) 

Instance Method

# pageController(\_:viewControllerForIdentifier:)

Returns a view controller the page controller uses for managing the specified identifier.

macOS 10.8+

``` source
@MainActor
optional func pageController(
    _ pageController: NSPageController,
    viewControllerForIdentifier identifier: NSPageController.ObjectIdentifier
) -> NSViewController
```

## Parameters 

`pageController`  

The page controller.

`identifier`  

The identifier for a view controller.

## Return Value

Returns the view controller for the specified identifier.

## Discussion

Your implementation of this method should return the requested view controller for the identifier or create and return a new view controller.

`NSPageController` will cache as many view controllers and views as necessary to maintain performance. This method is called whenever another instance is required.

The view controller may become the selectedViewController after a transition if necessary.

## See Also

### Managing View Controllers

func pageController(NSPageController, identifierFor: Any) -> NSPageController.ObjectIdentifier

Return the identifier of the view controller that owns a view to display the object.

func pageController(NSPageController, prepare: NSViewController, with: Any?)

Prepare the view controller and it’s view for drawing.

func pageController(NSPageController, frameFor: Any?) -> NSRect

Returns the frame appropriate for displaying the specified object.

typealias ObjectIdentifier

