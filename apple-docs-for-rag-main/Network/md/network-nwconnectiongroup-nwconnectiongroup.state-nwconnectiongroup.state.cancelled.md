

- Network
- NWConnectionGroup
- NWConnectionGroup.State
-  NWConnectionGroup.State.cancelled 

Case

# NWConnectionGroup.State.cancelled

The connection group has been canceled.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
case cancelled
```

## See Also

### States

case setup

You have not yet started the connection group.

case waiting(NWError)

The connection group is waiting for a network path change.

case ready

The connection group is joined, and ready to send and receive data.

case failed(NWError)

The connection group encountered a fatal error.

