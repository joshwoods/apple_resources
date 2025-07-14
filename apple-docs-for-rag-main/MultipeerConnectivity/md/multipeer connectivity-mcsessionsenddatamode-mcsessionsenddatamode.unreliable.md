

- Multipeer Connectivity
- MCSessionSendDataMode
-  MCSessionSendDataMode.unreliable 

Case

# MCSessionSendDataMode.unreliable

Messages to peers should be sent immediately without socket-level queueing. If a message cannot be sent immediately, it should be dropped. The order of messages is not guaranteed.

iOS 7.0+iPadOS 7.0+Mac Catalyst 13.1+macOS 10.10+tvOS 10.0+visionOS 1.0+

``` source
case unreliable
```

## Discussion

Use this message type for data that ceases to be relevant if delayed, such as real-time gaming data.

## See Also

### Constants

case reliable

The framework should guarantee delivery of each message, enqueueing and retransmitting data as needed, and ensuring in-order delivery.

