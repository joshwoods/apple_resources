

- AppKit
- NSPageControllerDelegate
-  pageController(\_:frameFor:) 

Instance Method

# pageController(\_:frameFor:)

Returns the frame appropriate for displaying the specified object.

macOS 10.8+

``` source
@MainActor
optional func pageController(
    _ pageController: NSPageController,
    frameFor object: Any?
) -> NSRect
```

## Parameters 

`pageController`  

The page controller.

`object`  

The object to display.

## Return Value

The frame appropriate for displaying `object`.

## Discussion

You only need to implement this if the view frame can differ between the page controller’s arrangedObjects.

This method must return immediately. Avoid file, network or any potentially blocking or lengthy work to provide an answer.

If this method is not implemented, all arrangedObjects are assumed to have the same frame as the `pageController` object’s current selectedViewController instance’s `view` or the bounds of `view` when selectedViewController is `nil`.

This method is only useful if pageController(_:identifierFor:) and pageController(_:viewControllerForIdentifier:) are implemented.

## See Also

### Managing View Controllers

func pageController(NSPageController, identifierFor: Any) -> NSPageController.ObjectIdentifier

Return the identifier of the view controller that owns a view to display the object.

func pageController(NSPageController, viewControllerForIdentifier: NSPageController.ObjectIdentifier) -> NSViewController

Returns a view controller the page controller uses for managing the specified identifier.

func pageController(NSPageController, prepare: NSViewController, with: Any?)

Prepare the view controller and it’s view for drawing.

typealias ObjectIdentifier

