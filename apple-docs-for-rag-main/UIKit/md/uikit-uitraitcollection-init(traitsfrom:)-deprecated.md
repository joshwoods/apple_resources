

- UIKit
- UITraitCollection
-  init(traitsFrom:) Deprecated

Initializer

# init(traitsFrom:)

Creates a trait collection that consists of traits merged from a specified array of trait collections.

iOS 8.0–17.0DeprecatediPadOS 8.0–17.0DeprecatedMac Catalyst 13.1–17.0DeprecatedtvOSDeprecatedvisionOS 1.0–1.0Deprecated

``` source
init(traitsFrom traitCollections: [UITraitCollection])
```

## Parameters 

`traitCollections`  

An array of UITraitCollection objects.

## Return Value

A new trait collection consisting of traits merged from a specified `traitCollections` array.

## Discussion

This method takes an array of one or more trait collections and merges them to create a new trait collection. If the array contains more than one element, the highest-indexed element that contains a given trait is used for that trait. For example, the following code snippet creates a trait collection with a *compact* horizontal size class, because the second element in the array overrides the first for that trait:

```
UITraitCollection *newHorizontalSizeClass1 = [UITraitCollection traitCollectionWithHorizontalSizeClass: UIUserInterfaceSizeClassRegular];
UITraitCollection *newHorizontalSizeClass2 = [UITraitCollection traitCollectionWithHorizontalSizeClass: UIUserInterfaceSizeClassCompact];
NSArray *traitArray = [NSArray arrayWithObjects: newHorizontalSizeClass1, newHorizontalSizeClass2, nil];
UITraitCollection *combinedTraits = [UITraitCollection traitCollectionWithTraitsFromCollections: traitArray];
```

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

