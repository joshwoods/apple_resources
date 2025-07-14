

- UIKit
- UIPresentationController
-  shouldRemovePresentersView 

Instance Property

# shouldRemovePresentersView

A Boolean value indicating whether the presenting view controller’s view should be removed when the presentation animations finish.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var shouldRemovePresentersView: Bool { get }
```

## Return Value

true if the view should be removed or false if it should not.

## Discussion

The default implementation of this method returns false. If you implement a presentation that does not cover the presenting view controller’s content entirely, override this method and return false.

If you override this method, do not call `super`.

## See Also

### Getting the presentation attributes

var presentationStyle: UIModalPresentationStyle

The presentation style of the presented view controller.

func adaptivePresentationStyle(for: UITraitCollection) -> UIModalPresentationStyle

Returns the presentation style to use for the specified set of traits.

var adaptivePresentationStyle: UIModalPresentationStyle

Returns the presentation style to use when the presented view controller becomes horizontally compact.

var shouldPresentInFullscreen: Bool

A Boolean value indicating whether the presentation covers the entire screen.

