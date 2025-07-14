

- AppKit
- NSAlertDelegate
-  alertShowHelp(\_:) 

Instance Method

# alertShowHelp(\_:)

Sent to the delegate when the user clicks the alert’s help button. The delegate causes help to be displayed for an alert, directly or indirectly.

macOS

``` source
@MainActor
optional func alertShowHelp(_ alert: NSAlert) -> Bool
```

## Return Value

true when the delegate displayed help directly, false otherwise. When false and the alert has a help anchor (helpAnchor), the application’s help manager displays help using the help anchor.

## Discussion

The delegate implements this method only to override the help-anchor lookup behavior.

## See Also

### Related Documentation

Sheet Programming Topics

var showsHelp: Bool

Specifies whether the alert has a help button.

Dialogs and Special Panels

