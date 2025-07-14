

- Core Telephony
-  CTSubscriberDelegate 

Protocol

# CTSubscriberDelegate

A protocol to handle changes to subscriber information.

iOS 12.1+iPadOS 12.1+

``` source
protocol CTSubscriberDelegate
```

## Topics

### Handling Token Updates

func subscriberTokenRefreshed(CTSubscriber)

Tells the delegate the subscriber’s token refreshed.

**Required**

## See Also

### Subscriber Information

class CTSubscriber

A cellular network subscriber.

class CTSubscriberInfo

An object that provides an array of cellular network subscribers.

