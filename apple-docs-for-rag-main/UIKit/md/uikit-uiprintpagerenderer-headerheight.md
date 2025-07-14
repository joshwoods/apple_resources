

- UIKit
- UIPrintPageRenderer
-  headerHeight 

Instance Property

# headerHeight

The height of the page header.

iOS 4.2+iPadOS 4.2+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var headerHeight: CGFloat { get set }
```

## Discussion

The header is measured in points from the top of printableRect and is above the content area. The default header height is 0.0.

## See Also

### Specifying header and footer heights

var footerHeight: CGFloat

The height of the page footer.

