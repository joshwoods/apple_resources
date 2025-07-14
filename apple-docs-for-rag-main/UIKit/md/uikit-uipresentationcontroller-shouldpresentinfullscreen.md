

- UIKit
- UIPresentationController
-  shouldPresentInFullscreen 

Instance Property

# shouldPresentInFullscreen

A Boolean value indicating whether the presentation covers the entire screen.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shouldPresentInFullscreen: Bool { get }
```

## Return Value

true if the presentation covers the screen or false if it covers all or part of the current view controller only.

## Discussion

The default implementation of this method returns true, indicating that the presentation covers the entire screen. You can override this method and return false to force the presentation to display only in the current context.

If you override this method, do not call `super`.

## See Also

### Getting the presentation attributes

var presentationStyle: UIModalPresentationStyle

The presentation style of the presented view controller.

func adaptivePresentationStyle(for: UITraitCollection) -> UIModalPresentationStyle

Returns the presentation style to use for the specified set of traits.

var adaptivePresentationStyle: UIModalPresentationStyle

Returns the presentation style to use when the presented view controller becomes horizontally compact.

var shouldRemovePresentersView: Bool

A Boolean value indicating whether the presenting view controller’s view should be removed when the presentation animations finish.

