

- Messages
- MSCriticalSMSMessenger
-  send(\_:to:) 

Instance Method

# send(\_:to:)

Sends a critical message to the specified recipient.

iOS 18.2+iPadOS 18.2+

``` source
func send(
    _ message: MSCriticalMessage,
    to recipient: MSRecipient
) async throws -> Bool
```

## Parameters 

`message`  

The message to send.

`recipient`  

The recipient to send the message to.

## Return Value

`true` if the message successfully sends.

## Mentioned in 

Sending SMS messages from an app

## Discussion

There’s no user interaction necessary for the framework to send this message. If the message sends successfully, the framework displays a notification indicating sending the message was successful. Upon error, this method throws a `MSCriticalMessagingError/errorDomain` error.

Note

The system may impose a rate limit on frequency of messages sent, if usage exceeds this limit the framework returns a MSCriticalMessagingError.sendFailed error.

