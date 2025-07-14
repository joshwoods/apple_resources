

- Network
- NWConnectionGroup
-  cancel() 

Instance Method

# cancel()

Cancels the connection group object and leaves the network group.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
final func cancel()
```

## See Also

### Managing Groups

var stateUpdateHandler: ((NWConnectionGroup.State) -> Void)?

A handler that receives connection group state updates.

enum State

States that indicate whether you can use a connection group to send and receive messages.

var state: NWConnectionGroup.State

The current state of the connection group.

