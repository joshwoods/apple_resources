

- AppKit
-  NSAlertDelegate 

Protocol

# NSAlertDelegate

A set of optional methods implemented by the delegate of an NSAlert object to respond to a user’s request for help.

macOS

``` source
protocol NSAlertDelegate : NSObjectProtocol
```

## Topics

### Displaying Help

func alertShowHelp(NSAlert) -> Bool

Sent to the delegate when the user clicks the alert’s help button. The delegate causes help to be displayed for an alert, directly or indirectly.

## Relationships

### Inherits From

- NSObjectProtocol

## See Also

### Alerts

class NSAlert

A modal dialog or sheet attached to a document window.

