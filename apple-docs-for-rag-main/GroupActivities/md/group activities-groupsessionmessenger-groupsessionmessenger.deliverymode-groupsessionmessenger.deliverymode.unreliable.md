

- Group Activities
- GroupSessionMessenger
- GroupSessionMessenger.DeliveryMode
-  GroupSessionMessenger.DeliveryMode.unreliable 

Case

# GroupSessionMessenger.DeliveryMode.unreliable

A best-effort attempt to deliver the message to known participants.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case unreliable
```

## Mentioned in 

Synchronizing data during a SharePlay activity

## Discussion

Use this approach when it’s okay to drop messages occasionally. Typically, you use this approach for messages you send frequently with similar information. For example, use it when the information in each new message replaces information in the preceding message.

This approach makes a best-effort attempt to deliver your messages to the known participants, and makes no guarantees on the delivery order of messages.

## See Also

### Getting the delivery mode options

case reliable

An attempt to ensure the delivery of messages to known participants.

