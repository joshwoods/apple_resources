

- UIKit
- UITraitCollection
-  init(horizontalSizeClass:) 

Initializer

# init(horizontalSizeClass:)

Creates a trait collection that contains only a specified horizontal size class.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
init(horizontalSizeClass: UIUserInterfaceSizeClass)
```

## Parameters 

`horizontalSizeClass`  

A UIUserInterfaceSizeClass value specifying the horizontal size class for the new trait collection.

## Return Value

A new trait collection containing only a specified horizontal size class trait.

## See Also

### Creating a trait collection

init()

Creates a trait collection whose traits are set to their default (unspecified) values.

init(userInterfaceIdiom: UIUserInterfaceIdiom)

Creates a trait collection that contains only a specified interface idiom.

init(verticalSizeClass: UIUserInterfaceSizeClass)

Creates a trait collection that contains only a specified vertical size class.

init(userInterfaceStyle: UIUserInterfaceStyle)

Creates a trait collection that contains only the specified user interface style trait.

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

