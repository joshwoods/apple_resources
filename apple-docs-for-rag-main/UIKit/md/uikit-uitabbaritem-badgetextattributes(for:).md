

- UIKit
- UITabBarItem
-  badgeTextAttributes(for:) 

Instance Method

# badgeTextAttributes(for:)

Returns the badge’s text attributes for the specified state.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func badgeTextAttributes(for state: UIControl.State) -> [NSAttributedString.Key : Any]?
```

## Parameters 

`state`  

The item’s state. For possible values, see UIControl.State.

## Discussion

Use this method to retrieve the attributes the item applies to its badge’s value for the specified state. For a list of attributes, see NSAttributedString.Key.

## See Also

### Configuring the item’s badge

var badgeValue: String?

The text that the item’s badge displays.

var badgeColor: UIColor?

The background color of the item’s badge.

func setBadgeTextAttributes([NSAttributedString.Key : Any]?, for: UIControl.State)

Registers text attributes that the badge uses for the specified state.

