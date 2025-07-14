

- Messages
- MSRecipient
-  init(phoneNumber:) 

Initializer

# init(phoneNumber:)

Creates a new critical message recipient with the provided phone number.

iOS 18.2+iPadOS 18.2+

``` source
init(phoneNumber: String)
```

## Parameters 

`phoneNumber`  

A phone number that conforms to the E.164 — international public telecommunication numbering plan, without any non-numeric characters such as parentheses, periods, dashes, or a plus character (+) that introduces a country code.

## Discussion

Use this method to create a new critical message recipient. When delivering messages, the framework displays the phone number you provide here.

Note

If the framework can’t send a message due to an invalid phone number, the framework throws and MSCriticalMessagingError.sendFailed error.

