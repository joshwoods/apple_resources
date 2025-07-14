

- UIKit
- UITraitCollection
-  init(userInterfaceStyle:) 

Initializer

# init(userInterfaceStyle:)

Creates a trait collection that contains only the specified user interface style trait.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+tvOS 10.0+visionOS 1.0+

``` source
init(userInterfaceStyle: UIUserInterfaceStyle)
```

## Parameters 

`userInterfaceStyle`  

The interface style for the trait collection. For a list of possible values, see UIUserInterfaceStyle.

## Return Value

A new trait collection containing only the interface style trait.

## See Also

### Creating a trait collection

init()

Creates a trait collection whose traits are set to their default (unspecified) values.

init(userInterfaceIdiom: UIUserInterfaceIdiom)

Creates a trait collection that contains only a specified interface idiom.

init(horizontalSizeClass: UIUserInterfaceSizeClass)

Creates a trait collection that contains only a specified horizontal size class.

init(verticalSizeClass: UIUserInterfaceSizeClass)

Creates a trait collection that contains only a specified vertical size class.

init(accessibilityContrast: UIAccessibilityContrast)

Creates a trait collection that contains only the specified accessibility contrast trait.

init(userInterfaceLevel: UIUserInterfaceLevel)

Creates a trait collection that contains only the specified user interface level trait.

init(legibilityWeight: UILegibilityWeight)

Creates a trait collection that contains only the specified legibility weight trait.

init(forceTouchCapability: UIForceTouchCapability)

Creates a trait collection that contains only a specified force touch capability trait.

init(displayScale: CGFloat)

Creates a trait collection that contains only a specified display scale.

init(displayGamut: UIDisplayGamut)

Creates a trait collection that contains only the specified display gamut trait.

init(layoutDirection: UITraitEnvironmentLayoutDirection)

Creates a trait collection that contains only the specified layout direction trait.

init(preferredContentSizeCategory: UIContentSizeCategory)

Creates a trait collection that contains only the specified content size category trait.

init(activeAppearance: UIUserInterfaceActiveAppearance)

Creates a trait collection that contains only the specified active appearance trait.

init(toolbarItemPresentationSize: UINSToolbarItemPresentationSize)

Creates a trait collection that contains only the specified toolbar item presentation size trait.

init?(coder: NSCoder)

Creates a trait collection from data in an unarchiver.

