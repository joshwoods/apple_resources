

- UIKit
- UIToolbar
-  compactAppearance 

Instance Property

# compactAppearance

The appearance settings to use for a compact-height toolbar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@NSCopying @MainActor
var compactAppearance: UIToolbarAppearance? { get set }
```

## Discussion

If the value of this property is `nil`, UIKit uses the same settings found in the standardAppearance property.

## See Also

### Customizing appearance

var standardAppearance: UIToolbarAppearance

The appearance settings to use for a standard-height toolbar.

var scrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a standard-height toolbar when the edge of scrollable content aligns with the edge of the toolbar.

var compactScrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a compact-height toolbar when the edge of any scrollable content aligns with the edge of a compact-height toolbar.

var isTranslucent: Bool

A Boolean value that indicates whether the toolbar is translucent.

Legacy customizations

Customize appearance information directly on the toolbar object.

