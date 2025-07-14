

- MailKit
- MEComposeSession
-  sessionID 

Instance Property

# sessionID

A unique identifier for the session.

macOS 12.0+

``` source
var sessionID: UUID { get }
```

## Discussion

A compose session’s identifier is only valid for the duration that Mail shows a compose window. If the user opens a compose window, saves it as a draft, and later reopens it, the compose session may have a different sessionID.

## See Also

### Managing Compose Sessions

func reload()

Refreshes the compose session with the extension’s new information.

