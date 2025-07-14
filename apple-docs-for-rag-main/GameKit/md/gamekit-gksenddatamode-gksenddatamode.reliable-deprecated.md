

- GameKit
- GKSendDataMode
-  GKSendDataMode.reliable Deprecated

Case

# GKSendDataMode.reliable

The data is sent continuously until it is successfully received by the intended recipients or the connection times out.

macOS 10.8–10.10DeprecatedtvOS 9.0–18.4DeprecatedvisionOS 1.0–1.0DeprecatedwatchOS 3.0–3.0Deprecated

``` source
case reliable
```

Deprecated

No longer supported

## Discussion

Reliable transmissions are delivered in the order they were sent. Use this when you need to guarantee delivery.

## See Also

### Constants

case unreliable

The data is sent once and is not sent again if a transmission error occurred.

Deprecated

