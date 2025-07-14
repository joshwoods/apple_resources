

- UIKit
- UIPresentationController
-  presentationStyle 

Instance Property

# presentationStyle

The presentation style of the presented view controller.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
@MainActor
var presentationStyle: UIModalPresentationStyle { get }
```

## Discussion

This property is set to the presentation style of the presented view controller. The presentation controller uses this style to determine the initial appearance of the presented content.

## See Also

### Getting the presentation attributes

func adaptivePresentationStyle(for: UITraitCollection) -> UIModalPresentationStyle

Returns the presentation style to use for the specified set of traits.

var adaptivePresentationStyle: UIModalPresentationStyle

Returns the presentation style to use when the presented view controller becomes horizontally compact.

var shouldPresentInFullscreen: Bool

A Boolean value indicating whether the presentation covers the entire screen.

var shouldRemovePresentersView: Bool

A Boolean value indicating whether the presenting view controller’s view should be removed when the presentation animations finish.

