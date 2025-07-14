

- UIKit
- UIBarButtonItemGroup
-  isDisplayingRepresentativeItem 

Instance Property

# isDisplayingRepresentativeItem

A Boolean value indicating whether the representative item is showing in place of the group’s items.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
var isDisplayingRepresentativeItem: Bool { get }
```

## Discussion

The value of this property is true when the representative item is being displayed in the shortcuts bar. The value is false when the individual bar button items are being displayed in the shortcuts bar.

## See Also

### Determining the group’s appearance

var isHidden: Bool

A Boolean that determines the visibility of the group.

