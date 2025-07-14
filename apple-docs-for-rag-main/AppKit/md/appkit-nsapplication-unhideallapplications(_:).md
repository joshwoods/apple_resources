

- AppKit
- NSApplication
-  unhideAllApplications(\_:) 

Instance Method

# unhideAllApplications(\_:)

Unhides all apps, including the receiver.

macOS

``` source
@MainActor
func unhideAllApplications(_ sender: Any?)
```

## Parameters 

`sender`  

The object that sent this message.

## Discussion

This action causes each app to order its windows to the front, which could obscure the currently active window in the active app.

## See Also

### Hiding Apps

func hideOtherApplications(Any?)

Hides all apps, except the receiver.

