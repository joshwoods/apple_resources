

- CallKit
- CXProvider
-  reportCall(with:endedAt:reason:) 

Instance Method

# reportCall(with:endedAt:reason:)

Reports to the provider that a call with the specified identifier ended at a given date for a particular reason.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func reportCall(
    with UUID: UUID,
    endedAt dateEnded: Date?,
    reason endedReason: CXCallEndedReason
)
```

## Parameters 

`UUID`  

The unique identifier of the call.

`dateEnded`  

The time at which the call ended.

If `nil`, the current time is used.

`endedReason`  

The reason that the call ended. For possible values, see CXCallEndedReason.

## See Also

### Reporting Calls

func reportNewIncomingCall(with: UUID, update: CXCallUpdate, completion: ((any Error)?) -> Void)

Reports a new incoming call with the specified unique identifier to the provider.

class func reportNewIncomingVoIPPushPayload([AnyHashable : Any], completion: (((any Error)?) -> Void)?)

Reports a new incoming call after your notification service extension decrypts a VoIP call request.

com.apple.developer.usernotifications.filtering

Enable receiving notifications without displaying the notification to the user.

func reportOutgoingCall(with: UUID, startedConnectingAt: Date?)

Reports to the provider that an outgoing call with the specified unique identifier started connecting at a particular time.

func reportOutgoingCall(with: UUID, connectedAt: Date?)

Reports to the provider that an outgoing call with the specified unique identifier finished connecting at a particular time.

func reportCall(with: UUID, updated: CXCallUpdate)

Reports to the provider that an active call updated its information.

