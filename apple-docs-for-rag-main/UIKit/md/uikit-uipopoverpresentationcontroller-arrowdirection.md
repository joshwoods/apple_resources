

- UIKit
- UIPopoverPresentationController
-  arrowDirection 

Instance Property

# arrowDirection

The arrow direction in use by the popover.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var arrowDirection: UIPopoverArrowDirection { get }
```

## Discussion

When the popover is onscreen, this property reflects the actual arrow direction. Before and after presentation, the value of this property is unknown.

## See Also

### Configuring the popover arrows

var permittedArrowDirections: UIPopoverArrowDirection

The arrow directions that you allow for the popover.

