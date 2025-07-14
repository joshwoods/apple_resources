

- UIKit
- UIAlertView
-  init(coder:) Deprecated

Initializer

# init(coder:)

Creates an alert view from data in an unarchiver.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
init?(coder: NSCoder)
```

## See Also

### Creating alert views

convenience init(title: String?, message: String?, delegate: Any?, cancelButtonTitle: String?)

Convenience method for initializing an alert view.

Deprecated

convenience init(title: String, message: String, delegate: (any UIAlertViewDelegate)?, cancelButtonTitle: String?, otherButtonTitles: String, String...)

Creates an alert view with the specified values.

Deprecated

init(frame: CGRect)

Creates an alert view with the specified frame.

Deprecated

