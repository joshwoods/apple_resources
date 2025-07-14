

- Network Extension
- NEVPNIKEv2DeadPeerDetectionRate
-  NEVPNIKEv2DeadPeerDetectionRate.none 

Case

# NEVPNIKEv2DeadPeerDetectionRate.none

Do not perform dead peer detection.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.11+tvOS 17.0+visionOS 1.0+

``` source
case none
```

## See Also

### Detection rates

case low

Run dead peer detection once every 30 minutes. If the peer does not respond, retry 5 times at 1 second intervals before declaring the peer dead and terminating the session.

case medium

Run dead peer detection once every 10 minutes. If the peer does not respond, retry 5 times at 1 second intervals before declaring the peer dead and terminating the session.

case high

Run dead peer detection once every 1 minute. If the peer does not respond, retry 5 times at 1 second intervals before declaring the peer dead and terminating the session.

