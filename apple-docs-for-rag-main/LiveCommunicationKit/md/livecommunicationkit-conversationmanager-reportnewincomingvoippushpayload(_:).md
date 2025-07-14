

- LiveCommunicationKit
- ConversationManager
-  reportNewIncomingVoIPPushPayload(\_:) 

Type Method

# reportNewIncomingVoIPPushPayload(\_:)

Reports a new incoming call after your notification service extension decrypts a VoIP call request.

iOS 17.4+iPadOS 17.4+Mac Catalyst 17.4+visionOS 1.1+watchOS 10.4+

``` source
final class func reportNewIncomingVoIPPushPayload(_ payload: [AnyHashable : Any]) async throws
```

## Parameters 

`payload`  

A dictionary containing additional data about the incoming call. All keys and values in the dictionary must implement the `NSSecureCoding` protocol.

## Discussion

Throws

When the system disallows a `Conversation`, an error is thrown that contains information about why it disallowed the `Conversation`.

