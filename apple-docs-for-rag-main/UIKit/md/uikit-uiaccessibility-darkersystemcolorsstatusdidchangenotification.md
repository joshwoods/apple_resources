

- UIKit
- UIAccessibility
-  darkerSystemColorsStatusDidChangeNotification 

Type Property

# darkerSystemColorsStatusDidChangeNotification

A notification that UIKit posts when the system’s Increase Contrast setting changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let darkerSystemColorsStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

## See Also

### Colors

static let grayscaleStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the system’s Grayscale setting changes.

static let invertColorsStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the settings for inverted colors change.

