

- UIKit
- UIPrintPageRenderer
-  footerHeight 

Instance Property

# footerHeight

The height of the page footer.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var footerHeight: CGFloat { get set }
```

## Discussion

The footer is measured in points from the bottom of printableRect and is below the content area. The default footer height is 0.0

## See Also

### Specifying header and footer heights

var headerHeight: CGFloat

The height of the page header.

