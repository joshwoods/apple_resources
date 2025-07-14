

- UIKit
- UITabBarItemAppearance
-  init(style:) 

Initializer

# init(style:)

Creates an appearance object with appropriate default values for a tab bar, displaying its items with the specified layout style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
init(style: UITabBarItemAppearance.Style)
```

## Parameters 

`style`  

The layout style for the appearance attributes. UIKit uses this value to configure the default appearance attributes. For a list of possible values, see UITabBarItemAppearance.Style.

## Return Value

A new appearance object containing appropriate default values for the specified layout style.

## See Also

### Creating a tab bar item appearance object

convenience init()

Creates an appearance object with default values for a stacked tab bar item.

init(coder: NSCoder)

Creates an appearance object from data in an unarchiver.

