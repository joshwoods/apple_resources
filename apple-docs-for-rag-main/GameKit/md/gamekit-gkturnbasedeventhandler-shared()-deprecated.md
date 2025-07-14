

- GameKit
- GKTurnBasedEventHandler
-  shared() Deprecated

Type Method

# shared()

Returns the shared instance of the event handler.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
class func shared() -> GKTurnBasedEventHandler
```

## Return Value

An event handler object.

## Discussion

Your game never directly creates a GKTurnBasedEventHandler object. Instead, retrieve the shared instance using this class method.

