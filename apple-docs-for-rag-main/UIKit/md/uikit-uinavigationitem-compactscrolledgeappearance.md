

- UIKit
- UINavigationItem
-  compactScrollEdgeAppearance 

Instance Property

# compactScrollEdgeAppearance

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+tvOS 15.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var compactScrollEdgeAppearance: UINavigationBarAppearance? { get set }
```

## Discussion

When a compact-height navigation bar displays the top navigation item, the appearance setting in this property overrides the settings in the compactScrollEdgeAppearance property of UINavigationBar.

Use this property to apply appearance settings to the navigation bar based on the navigation item stored in the topItem property. If the top item’s compactScrollEdgeAppearance property is `nil`, UIKit uses the navigation bar’s compact scroll edge appearance.

## See Also

### Overriding the navigation bar’s appearance settings

var standardAppearance: UINavigationBarAppearance?

The appearance settings for a standard-height navigation bar.

var compactAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a standard-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

