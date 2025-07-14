

- GameKit
- GKSession
-  init(sessionID:displayName:sessionMode:) Deprecated

Initializer

# init(sessionID:displayName:sessionMode:)

Initializes and returns a newly allocated session.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–2.0Deprecated

``` source
init!(
    sessionID: String!,
    displayName name: String!,
    sessionMode mode: GKSessionMode
)
```

Deprecated

No longer available

## Parameters 

`sessionID`  

A unique string that identifies your application. Your `sessionID` should be the short name of an approved Bonjour service type. If `nil`, the session uses the application’s bundle identifier to create a `sessionID` string.

`name`  

A string identifying the user to display to other peers. If `nil`, the session uses the device name.

`mode`  

The mode the session should run in. See GKSessionMode for possible values.

## Return Value

An initialized session object, or `nil` if an error occurred.

## Discussion

Only sessions running with the same `sessionID` are visible to your session.

