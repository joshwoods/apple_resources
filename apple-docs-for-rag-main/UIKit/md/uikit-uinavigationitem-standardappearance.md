

- UIKit
- UINavigationItem
-  standardAppearance 

Instance Property

# standardAppearance

The appearance settings for a standard-height navigation bar.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+

``` source
@NSCopying @MainActor
var standardAppearance: UINavigationBarAppearance? { get set }
```

## Discussion

When the navigation bar displays the current navigation item, the appearance settings in this property override the settings provided by the standardAppearance property of UINavigationBar.

Use this property to apply appearance settings to the navigation bar based on the navigation item stored in the topItem property. If the top item’s standardAppearance property is `nil`, UIKit uses the navigation bar’s appearance.

## See Also

### Overriding the navigation bar’s appearance settings

var compactAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a standard-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var compactScrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

