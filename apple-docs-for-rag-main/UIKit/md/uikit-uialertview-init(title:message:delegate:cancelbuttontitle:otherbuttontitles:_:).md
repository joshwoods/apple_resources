

- UIKit
- UIAlertView
-  init(title:message:delegate:cancelButtonTitle:otherButtonTitles:\_:) 

Initializer

# init(title:message:delegate:cancelButtonTitle:otherButtonTitles:\_:)

Creates an alert view with the specified values.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst

``` source
@MainActor @preconcurrency
convenience init(
    title: String,
    message: String,
    delegate: (any UIAlertViewDelegate)?,
    cancelButtonTitle: String?,
    otherButtonTitles firstButtonTitle: String,
    _ moreButtonTitles: String...
)
```

## See Also

### Creating alert views

convenience init(title: String?, message: String?, delegate: Any?, cancelButtonTitle: String?)

Convenience method for initializing an alert view.

Deprecated

init(frame: CGRect)

Creates an alert view with the specified frame.

Deprecated

init?(coder: NSCoder)

Creates an alert view from data in an unarchiver.

Deprecated

