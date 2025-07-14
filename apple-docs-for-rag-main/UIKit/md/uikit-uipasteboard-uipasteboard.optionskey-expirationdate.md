

- UIKit
- UIPasteboard
- UIPasteboard.OptionsKey
-  expirationDate 

Type Property

# expirationDate

The time and date that you want the system to remove the pasteboard items from the pasteboard.

iOS 10.0+iPadOS 10.0+Mac Catalyst 13.1+visionOS 1.0+

``` source
static let expirationDate: UIPasteboard.OptionsKey
```

## Discussion

Specify the date and time as an NSDate value.

## See Also

### Constants

static let localOnly: UIPasteboard.OptionsKey

A Boolean value that specifies that the pasteboard items should not be available to other devices through the Handoff feature.

