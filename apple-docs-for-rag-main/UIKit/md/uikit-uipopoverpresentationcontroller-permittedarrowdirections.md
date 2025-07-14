

- UIKit
- UIPopoverPresentationController
-  permittedArrowDirections 

Instance Property

# permittedArrowDirections

The arrow directions that you allow for the popover.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var permittedArrowDirections: UIPopoverArrowDirection { get set }
```

## Discussion

Prior to displaying the popover, set this property to the arrow directions that you allow for your popover. The actual arrow direction in use by the popover is stored in the arrowDirection property.

The default value of this property is any.

## See Also

### Configuring the popover arrows

var arrowDirection: UIPopoverArrowDirection

The arrow direction in use by the popover.

