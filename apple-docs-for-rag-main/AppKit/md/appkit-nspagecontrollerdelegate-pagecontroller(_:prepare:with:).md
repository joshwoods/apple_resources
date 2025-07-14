

- AppKit
- NSPageControllerDelegate
-  pageController(\_:prepare:with:) 

Instance Method

# pageController(\_:prepare:with:)

Prepare the view controller and it’s view for drawing.

macOS 10.8+

``` source
@MainActor
optional func pageController(
    _ pageController: NSPageController,
    prepare viewController: NSViewController,
    with object: Any?
)
```

## Parameters 

`pageController`  

The page controller.

`viewController`  

The view controller to prepare for drawing. You should setup the data sources and perform layout.

`object`  

The object to display.

## Discussion

If this method is not implemented, then `viewController` object’s `representedObject` is set to the object.

Note

This method is called on the main thread and should return immediately. The view will be asked to draw on a background thread and must support background drawing.

This method is only useful if pageController(_:identifierFor:) and pageController(_:prepare:with:) are implemented.

## See Also

### Managing View Controllers

func pageController(NSPageController, identifierFor: Any) -> NSPageController.ObjectIdentifier

Return the identifier of the view controller that owns a view to display the object.

func pageController(NSPageController, viewControllerForIdentifier: NSPageController.ObjectIdentifier) -> NSViewController

Returns a view controller the page controller uses for managing the specified identifier.

func pageController(NSPageController, frameFor: Any?) -> NSRect

Returns the frame appropriate for displaying the specified object.

typealias ObjectIdentifier

