

- GameKit
- GKSession
-  isAvailable Deprecated

Instance Property

# isAvailable

A Boolean value that determines whether or not the session wants to connect to new peers.

macOS 10.8–10.10DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 2.0–2.0Deprecated

``` source
var isAvailable: Bool { get set }
```

## Discussion

When isAvailable is true, the session is visible to other peers based on its sessionMode property. When isAvailable is set to false, it remains connected to peers, but is no longer visible to nonconnected peers. The default is false.

Typically, your application configures the session object with a delegate and data receiver, and then sets isAvailable to true. When the delegate finishes connecting to peers, it should set the session’s isAvailable property to false.

