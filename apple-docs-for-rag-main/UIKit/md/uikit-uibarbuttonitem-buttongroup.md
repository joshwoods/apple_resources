

- UIKit
- UIBarButtonItem
-  buttonGroup 

Instance Property

# buttonGroup

The group that the button belongs to.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+

``` source
@MainActor
weak var buttonGroup: UIBarButtonItemGroup? { get }
```

## Discussion

This property contains the group to which the item belongs. This property is configured automatically when you add the bar button item to a UIBarButtonItemGroup object. If the item isn’t associated with a bar button item group, this property is `nil`.

