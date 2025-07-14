

- UIKit
- UIBarButtonItemGroup
-  alwaysAvailable 

Instance Property

# alwaysAvailable

A Boolean value that determines whether the group is always available through the UI.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+visionOS 1.0+

``` source
@MainActor
var alwaysAvailable: Bool { get set }
```

## Discussion

Set this property to true to ensure that the functionality in this group is available to people regardless of the customization of the groups.

When the value is true, UIKit places the items in this group in the overflow menu for the UIUserInterfaceIdiom.phone and UIUserInterfaceIdiom.pad idioms. This property doesn’t have an effect for the UIUserInterfaceIdiom.mac idiom.

## See Also

### Configuring the group

var barButtonItems: [UIBarButtonItem]

The bar button items to display on the bar.

var representativeItem: UIBarButtonItem?

The item to display for a group when space is constrained.

