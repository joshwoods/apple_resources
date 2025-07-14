

- UIKit
- UIAccessibility
-  invertColorsStatusDidChangeNotification 

Type Property

# invertColorsStatusDidChangeNotification

A notification that UIKit posts when the settings for inverted colors change.

iOS 6.0+iPadOS 6.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let invertColorsStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

Use the isInvertColorsEnabled function to determine whether the settings for inverted colors are in an enabled state.

## See Also

### Colors

static let darkerSystemColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Increase Contrast setting changes.

static let grayscaleStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Grayscale setting changes.

