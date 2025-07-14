

- Messages
- MSCriticalSMSMessenger
-  checkAuthorizationStatus(for:) 

Instance Method

# checkAuthorizationStatus(for:)

Confirms the current authorization status for sending critical messages from this app.

iOS 18.2+iPadOS 18.2+

``` source
func checkAuthorizationStatus(for recipients: [MSRecipient]) async throws -> [MSRecipient : MSCriticalMessagingAuthorizationStatus]
```

## Parameters 

`recipients`  

An array of recipients to check the authorization status for.

## Return Value

A dictionary that maps recipients to their corresponding authorization status.

## Mentioned in 

Sending SMS messages from an app

## Discussion

You can call this method multiple times to check the authorization status for multiple recipients. Upon an error, the method throws an error of \`MSCriticalMessagingErrorDomain\`\`.

