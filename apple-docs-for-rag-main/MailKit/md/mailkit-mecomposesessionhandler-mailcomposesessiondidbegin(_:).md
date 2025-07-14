

- MailKit
- MEComposeSessionHandler
-  mailComposeSessionDidBegin(\_:) 

Instance Method

# mailComposeSessionDidBegin(\_:)

Informs the handler when the user opens a compose window.

macOS 12.0+

``` source
@MainActor
func mailComposeSessionDidBegin(_ session: MEComposeSession)
```

**Required**

## Parameters 

`session`  

The compose session that corresponds to the message the user is composing.

## See Also

### Handling Compose Sessions

class MEComposeSession

An object that represents a single mail compose window.

func mailComposeSessionDidEnd(MEComposeSession)

Informs the handler when the user closes a compose window.

**Required**

struct MEComposeSessionError

An error that indicates the compose session is in an erroneous state.

