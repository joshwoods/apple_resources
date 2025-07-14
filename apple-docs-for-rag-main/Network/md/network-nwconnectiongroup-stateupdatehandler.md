

- Network
- NWConnectionGroup
-  stateUpdateHandler 

Instance Property

# stateUpdateHandler

A handler that receives connection group state updates.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
@preconcurrency
final var stateUpdateHandler: ((NWConnectionGroup.State) -> Void)? { get set }
```

## See Also

### Managing Groups

enum State

States that indicate whether you can use a connection group to send and receive messages.

var state: NWConnectionGroup.State

The current state of the connection group.

func cancel()

Cancels the connection group object and leaves the network group.

