

- UIKit
- UITabBarItemAppearance
-  configureWithDefault(for:) 

Instance Method

# configureWithDefault(for:)

Configures the tab bar item appearance object with appropriate values for the specified style.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@MainActor
func configureWithDefault(for style: UITabBarItemAppearance.Style)
```

## Parameters 

`style`  

The layout style for the appearance attributes. UIKit configures the object with the default appearance attributes for the specified style. For a list of possible values, see UITabBarItemAppearance.Style.

## See Also

### Resetting the appearance properties

enum Style

Constants indicating the layout of a tab bar item’s content.

