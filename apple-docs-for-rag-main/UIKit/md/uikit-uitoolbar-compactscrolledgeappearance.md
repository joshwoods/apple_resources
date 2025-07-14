

- UIKit
- UIToolbar
-  compactScrollEdgeAppearance 

Instance Property

# compactScrollEdgeAppearance

The appearance settings for a compact-height toolbar when the edge of any scrollable content aligns with the edge of a compact-height toolbar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var compactScrollEdgeAppearance: UIToolbarAppearance? { get set }
```

## Discussion

When a navigation controller contains a toolbar and a scroll view, part of the scroll view’s content appears underneath the toolbar. If the edge of the scrolled content reaches the toolbar, UIKit applies the appearance settings in this property.

This property applies to compact-height toolbars. If the value of this property is `nil`, UIKit uses the value of the scrollEdgeAppearance property. If no navigation controller manages your toolbar, UIKit ignores this property and uses the value of the compactAppearance property.

## See Also

### Customizing appearance

var standardAppearance: UIToolbarAppearance

The appearance settings to use for a standard-height toolbar.

var compactAppearance: UIToolbarAppearance?

The appearance settings to use for a compact-height toolbar.

var scrollEdgeAppearance: UIToolbarAppearance?

The appearance settings for a standard-height toolbar when the edge of scrollable content aligns with the edge of the toolbar.

var isTranslucent: Bool

A Boolean value that indicates whether the toolbar is translucent.

Legacy customizations

Customize appearance information directly on the toolbar object.

