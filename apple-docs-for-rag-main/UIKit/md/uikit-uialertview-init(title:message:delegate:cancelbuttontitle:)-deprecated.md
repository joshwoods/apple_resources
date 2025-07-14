

- UIKit
- UIAlertView
-  init(title:message:delegate:cancelButtonTitle:) Deprecated

Initializer

# init(title:message:delegate:cancelButtonTitle:)

Convenience method for initializing an alert view.

iOS 2.0–9.0DeprecatediPadOS 2.0–9.0DeprecatedMac Catalyst 13.1–13.1Deprecated

``` source
@MainActor
convenience init(
    title: String?,
    message: String?,
    delegate: Any?,
    cancelButtonTitle: String?
)
```

## Parameters 

`title`  

The string that appears in the receiver’s title bar.

`message`  

Descriptive text that provides more details than the title.

`delegate`  

The receiver’s delegate or `nil` if it doesn’t have a delegate.

`cancelButtonTitle`  

The title of the cancel button or `nil` if there’s no cancel button.

Using this argument is equivalent to setting the cancel button index to the value returned by invoking addButton(withTitle:) specifying this title.

## Return Value

Newly initialized alert view.

## See Also

### Creating alert views

convenience init(title: String, message: String, delegate: (any UIAlertViewDelegate)?, cancelButtonTitle: String?, otherButtonTitles: String, String...)

Creates an alert view with the specified values.

Deprecated

init(frame: CGRect)

Creates an alert view with the specified frame.

Deprecated

init?(coder: NSCoder)

Creates an alert view from data in an unarchiver.

Deprecated

