

- XPC
- XPCPeerHandler
-  handleCancellation(error:) 

Instance Method

# handleCancellation(error:)

A closure the system invokes when it cancels a session with a client.

Mac Catalyst 17.0+macOS 14.0+

``` source
func handleCancellation(error: XPCRichError)
```

**Required** Default implementation provided.

## Parameters 

`error`  

A description of the reason for the session’s cancellation.

## Default Implementations

### XPCPeerHandler Implementations

func handleCancellation(error: XPCRichError)

A closure the system invokes when it cancels a session with a client.

