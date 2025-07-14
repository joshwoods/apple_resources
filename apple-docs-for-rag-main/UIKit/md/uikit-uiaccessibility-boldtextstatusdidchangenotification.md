

- UIKit
- UIAccessibility
-  boldTextStatusDidChangeNotification 

Type Property

# boldTextStatusDidChangeNotification

A notification that UIKit posts when the system’s Bold Text setting changes.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+tvOSvisionOS 1.0+

``` source
nonisolated
static let boldTextStatusDidChangeNotification: NSNotification.Name
```

## Discussion

This notification doesn’t include a parameter. Observe this notification using the default notification center.

## See Also

### Text

static let closedCaptioningStatusDidChangeNotification: NSNotification.Name

A notification that UIKit posts when the setting for Closed Captions + SDH changes.

