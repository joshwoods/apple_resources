

- CallKit
- CXProvider
-  reportNewIncomingVoIPPushPayload(\_:completion:) 

Type Method

# reportNewIncomingVoIPPushPayload(\_:completion:)

Reports a new incoming call after your notification service extension decrypts a VoIP call request.

iOS 14.5+iPadOS 14.5+Mac Catalyst 14.5+visionOS 1.0+

``` source
class func reportNewIncomingVoIPPushPayload(
    _ dictionaryPayload: [AnyHashable : Any],
    completion: (((any Error)?) -> Void)? = nil
)
```

``` source
class func reportNewIncomingVoIPPushPayload(_ dictionaryPayload: [AnyHashable : Any]) async throws
```

## Parameters 

`dictionaryPayload`  

A dictionary containing additional data about the incoming call. All keys and values in the dictionary must implement the NSSecureCoding protocol.

`completion`  

A block that CallKit executes after allowing or disallowing the call. CallKit executes the block on a private serial queue. The completion handler takes the following parameter:

`error`  
When the system disallows a call, it sets this parameter to an error object that contains information about why it disallowed the call; otherwise it’s `nil`.

## Mentioned in 

Sending End-to-End Encrypted VoIP Calls

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
class func reportNewIncomingVoIPPushPayload(_ dictionaryPayload: [AnyHashable : Any]) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

Call this method when your notification service extension receives an encrypted VoIP call request. The system then launches your app and calls your pushRegistry(_:didReceiveIncomingPushWith:for:completion:) method. From this point, the app handles the call just like any incoming VoIP call. For more information, see Sending End-to-End Encrypted VoIP Calls.

To call this method, your notification service extension must have the com.apple.developer.usernotifications.filtering entitlement.

Important

Only call this method when your server can’t determine whether an outgoing notification is a request for a VoIP call or some other data (such as a text message) due to metadata encryption. If your server knows that the outgoing content is a VoIP call, send a voIP push notification instead. For more information, see PushKit.

## See Also

### Reporting Calls

func reportNewIncomingCall(with: UUID, update: CXCallUpdate, completion: ((any Error)?) -> Void)

Reports a new incoming call with the specified unique identifier to the provider.

com.apple.developer.usernotifications.filtering

Enable receiving notifications without displaying the notification to the user.

func reportOutgoingCall(with: UUID, startedConnectingAt: Date?)

Reports to the provider that an outgoing call with the specified unique identifier started connecting at a particular time.

func reportOutgoingCall(with: UUID, connectedAt: Date?)

Reports to the provider that an outgoing call with the specified unique identifier finished connecting at a particular time.

func reportCall(with: UUID, updated: CXCallUpdate)

Reports to the provider that an active call updated its information.

func reportCall(with: UUID, endedAt: Date?, reason: CXCallEndedReason)

Reports to the provider that a call with the specified identifier ended at a given date for a particular reason.

