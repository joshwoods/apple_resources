

- CallKit
- CXProvider
-  reportCall(with:updated:) 

Instance Method

# reportCall(with:updated:)

Reports to the provider that an active call updated its information.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func reportCall(
    with UUID: UUID,
    updated update: CXCallUpdate
)
```

## Parameters 

`UUID`  

The unique identifier of the call.

`update`  

The updated information.

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

func reportCall(with: UUID, endedAt: Date?, reason: CXCallEndedReason)

Reports to the provider that a call with the specified identifier ended at a given date for a particular reason.

