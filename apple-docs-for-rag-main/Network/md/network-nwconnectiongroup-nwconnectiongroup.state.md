

- Network
- NWConnectionGroup
-  NWConnectionGroup.State 

Enumeration

# NWConnectionGroup.State

States that indicate whether you can use a connection group to send and receive messages.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
enum State
```

## Topics

### States

case setup

You have not yet started the connection group.

case waiting(NWError)

The connection group is waiting for a network path change.

case ready

The connection group is joined, and ready to send and receive data.

case failed(NWError)

The connection group encountered a fatal error.

case cancelled

The connection group has been canceled.

## Relationships

### Conforms To

- Equatable
- Sendable

## See Also

### Managing Groups

var stateUpdateHandler: ((NWConnectionGroup.State) -> Void)?

A handler that receives connection group state updates.

var state: NWConnectionGroup.State

The current state of the connection group.

func cancel()

Cancels the connection group object and leaves the network group.

