

- UIKit
- UITabBarItem
-  setBadgeTextAttributes(\_:for:) 

Instance Method

# setBadgeTextAttributes(\_:for:)

Registers text attributes that the badge uses for the specified state.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
@MainActor
func setBadgeTextAttributes(
    _ textAttributes: [NSAttributedString.Key : Any]?,
    for state: UIControl.State
)
```

## Parameters 

`textAttributes`  

A dictionary of text attributes. For a list of possible attributes, see NSAttributedString.Key.

`state`  

The item’s state. For possible values, see UIControl.State.

## Discussion

The setTitleTextAttributes(_:for:) method allows you to customize the appearance of the item’s title. Use this method to apply similar customizations to the badge’s value to achieve a consistent appearance.

## See Also

### Configuring the item’s badge

var badgeValue: String?

The text that the item’s badge displays.

var badgeColor: UIColor?

The background color of the item’s badge.

func badgeTextAttributes(for: UIControl.State) -> [NSAttributedString.Key : Any]?

Returns the badge’s text attributes for the specified state.

