

- Group Activities
- GroupSessionMessenger
- GroupSessionMessenger.DeliveryMode
-  GroupSessionMessenger.DeliveryMode.reliable 

Case

# GroupSessionMessenger.DeliveryMode.reliable

An attempt to ensure the delivery of messages to known participants.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+macOS 13.0+tvOS 16.0+visionOS 1.0+

``` source
case reliable
```

## Mentioned in 

Synchronizing data during a SharePlay activity

## Discussion

Use this approach to send messages that are critical to the experience you create. The GroupSessionMessenger enqueues a message until it is successfully transmitted to all known participants. The system doesn’t guarantee delivery to participants who join a group session after you send a message, or who leave the group prior to delivery.

## See Also

### Getting the delivery mode options

case unreliable

A best-effort attempt to deliver the message to known participants.

