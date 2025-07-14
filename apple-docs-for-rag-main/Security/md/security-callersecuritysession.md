

- Security
-  callerSecuritySession 

Global Variable

# callerSecuritySession

A value that is a placeholder for the caller’s session.

Mac Catalyst 13.0+macOS 10.0+

``` source
var callerSecuritySession: SecuritySessionId { get }
```

## Discussion

When you provide this value as the `session` input to the SessionGetInfo(_:_:_:) function, the function will return the actual session ID via the `sessionId` output.

