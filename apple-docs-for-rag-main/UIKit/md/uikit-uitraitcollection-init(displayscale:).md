

- UIKit
- UITraitCollection
-  init(displayScale:) 

Initializer

# init(displayScale:)

Creates a trait collection that contains only a specified display scale.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
init(displayScale scale: CGFloat)
```

## Parameters 

`scale`  

The display scale for the new trait collection. Use `1.0` to specify a non-Retina display scale, and a value of `2.0` or greater to specify a Retina display scale.

## Return Value

A new trait collection containing only a specified display scale trait.

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

