

- UIKit
- UINavigationBar
-  prefersLargeTitles 

Instance Property

# prefersLargeTitles

A Boolean value that indicates whether the title displays in a large format.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
@MainActor
var prefersLargeTitles: Bool { get set }
```

## Discussion

When this property is set to true, the navigation bar allows the title to be displayed out-of-line and using a larger font. The navigation item used to build the bar must specify whether it wants its title displayed in the large or small format. Use the largeTitleDisplayMode property to configure the title’s appearance.

When the property is set to false, the navigation bar displays the title inline with the other bar button items.

## See Also

### Customizing the bar’s appearance

var standardAppearance: UINavigationBarAppearance

The appearance settings for a standard-height navigation bar.

var compactAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar.

var scrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for the navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var compactScrollEdgeAppearance: UINavigationBarAppearance?

The appearance settings for a compact-height navigation bar when the edge of scrollable content aligns with the edge of the navigation bar.

var isTranslucent: Bool

A Boolean value that indicates whether the navigation bar is translucent.

Legacy customizations

Customize appearance information directly on the navigation bar object.

