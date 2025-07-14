

- Multipeer Connectivity
- MCSessionSendDataMode
-  MCSessionSendDataMode.reliable 

Case

# MCSessionSendDataMode.reliable

The framework should guarantee delivery of each message, enqueueing and retransmitting data as needed, and ensuring in-order delivery.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
case reliable
```

## Discussion

Use this message type for application-critical data.

## See Also

### Constants

case unreliable

Messages to peers should be sent immediately without socket-level queueing. If a message cannot be sent immediately, it should be dropped. The order of messages is not guaranteed.

