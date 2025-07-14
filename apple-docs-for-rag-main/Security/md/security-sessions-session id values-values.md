

- Security
- Sessions
-  Session ID Values 

API Collection

# Session ID Values

Use these values as placeholders for specific sessions.

## Discussion

You can use these values as the `session` input to the SessionGetInfo(_:_:_:) function as a stand-in for specific sessions when you don’t already know the ID for that session. They are *not* returned in the `sessionId` output of that function. Instead, you receive the actual session ID.

## Topics

### Constants

var callerSecuritySession: SecuritySessionId

A value that is a placeholder for the caller’s session.

var noSecuritySession: SecuritySessionId

Not a valid session.

