

- UIKit
- UIPopoverBackgroundViewMethods
-  arrowHeight() 

Type Method

# arrowHeight()

The height of the arrow (measured in points) from its base to its tip.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+tvOS 9.0+

``` source
static func arrowHeight() -> CGFloat
```

**Required**

## Discussion

Use this method to return the height of the arrow used by your popover background content. The arrow height must be the same for all possible directions and that height must not change.

## See Also

### Accessing the arrow metrics

static func arrowBase() -> CGFloat

The width of the arrow triangle at its base.

**Required**

