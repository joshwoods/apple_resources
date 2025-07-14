

- AppKit
- NSPageControllerDelegate
-  pageController(\_:identifierFor:) 

Instance Method

# pageController(\_:identifierFor:)

Return the identifier of the view controller that owns a view to display the object.

macOS 10.8+

``` source
@MainActor
optional func pageController(
    _ pageController: NSPageController,
    identifierFor object: Any
) -> NSPageController.ObjectIdentifier
```

## Parameters 

`pageController`  

The page controller.

`object`  

The object to display.

## Return Value

Returns a string identifier for the view controller for the specified object.

## Discussion

If `pageController` does not have an unused view controller for this identifier, the you will be asked to create one via pageController(_:viewControllerForIdentifier:).

## See Also

### Managing View Controllers

func pageController(NSPageController, viewControllerForIdentifier: NSPageController.ObjectIdentifier) -> NSViewController

Returns a view controller the page controller uses for managing the specified identifier.

func pageController(NSPageController, prepare: NSViewController, with: Any?)

Prepare the view controller and it’s view for drawing.

func pageController(NSPageController, frameFor: Any?) -> NSRect

Returns the frame appropriate for displaying the specified object.

typealias ObjectIdentifier

