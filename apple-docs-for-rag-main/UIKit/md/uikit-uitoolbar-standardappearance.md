

- UIKit
- UIToolbar
-  standardAppearance 

Instance Property

# standardAppearance

The appearance settings to use for a standard-height toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying @MainActor
var standardAppearance: UIToolbarAppearance { get set }
```

## Discussion

The default value of this property is an appearance object containing the system’s default appearance settings.

## See Also

### Customizing appearance

var compactAppearance: UIToolbarAppearance?

The appearance settings to use for a compact-height toolbar.

var scrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a standard-height toolbar when the edge of scrollable content aligns with the edge of the toolbar.

var compactScrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a compact-height toolbar when the edge of any scrollable content aligns with the edge of a compact-height toolbar.

var isTranslucent: Bool

A Boolean value that indicates whether the toolbar is translucent.

Legacy customizations

Customize appearance information directly on the toolbar object.

