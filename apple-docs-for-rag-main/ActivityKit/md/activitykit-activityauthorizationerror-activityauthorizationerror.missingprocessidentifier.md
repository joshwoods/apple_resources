

- ActivityKit
- ActivityAuthorizationError
-  ActivityAuthorizationError.missingProcessIdentifier 

Case

# ActivityAuthorizationError.missingProcessIdentifier

The process that tried to start the Live Activity is missing a process identifier.

iOS 16.1+iPadOS 16.1+

``` source
case missingProcessIdentifier
```

## See Also

### Error codes

case attributesTooLarge

The provided Live Activity attributes exceeded the maximum size of 4KB.

case denied

A person deactivated Live Activities in Settings.

case globalMaximumExceeded

The device reached the maximum number of ongoing Live Activities.

case malformedActivityIdentifier

The provided activity identifier is malformed.

case persistenceFailure

The system couldn’t persist the Live Activity.

case reconnectNotPermitted

The process that tried to recreate the Live Activity is not the process that originally created the Live Activity.

case targetMaximumExceeded

The app has already started the maximum number of concurrent Live Activities.

case unentitled

The app doesn’t have the required entitlement to start a Live Activity.

case unsupported

The device doesn’t support Live Activities.

case unsupportedTarget

The app doesn’t have the required entitlement to start a Live Activities.

case visibility

The app tried to start the Live Activity while it was in the background.

