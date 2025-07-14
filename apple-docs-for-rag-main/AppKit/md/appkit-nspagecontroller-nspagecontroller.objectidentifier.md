

- AppKit
- NSPageController
-  NSPageController.ObjectIdentifier 

Type Alias

# NSPageController.ObjectIdentifier

macOS

``` source
typealias ObjectIdentifier = String
```

## See Also

### Managing View Controllers

func pageController(NSPageController, identifierFor: Any) -> NSPageController.ObjectIdentifier

Return the identifier of the view controller that owns a view to display the object.

func pageController(NSPageController, viewControllerForIdentifier: NSPageController.ObjectIdentifier) -> NSViewController

Returns a view controller the page controller uses for managing the specified identifier.

func pageController(NSPageController, prepare: NSViewController, with: Any?)

Prepare the view controller and it’s view for drawing.

func pageController(NSPageController, frameFor: Any?) -> NSRect

Returns the frame appropriate for displaying the specified object.

