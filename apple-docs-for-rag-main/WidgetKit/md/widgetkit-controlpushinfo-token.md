

- WidgetKit
- ControlPushInfo
-  token 

Instance Property

# token

A unique push token that may be used to deliver updates for this control.

iOS 18.0+iPadOS 18.0+Mac Catalyst 18.0+

``` source
let token: Data
```

## Discussion

This token is valid until told otherwise through the pushTokensDidChange(controls:) method on your push handler.

