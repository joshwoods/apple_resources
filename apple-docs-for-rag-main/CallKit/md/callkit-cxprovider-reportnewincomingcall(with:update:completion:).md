

- CallKit
- CXProvider
-  reportNewIncomingCall(with:update:completion:) 

Instance Method

# reportNewIncomingCall(with:update:completion:)

Reports a new incoming call with the specified unique identifier to the provider.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
func reportNewIncomingCall(
    with UUID: UUID,
    update: CXCallUpdate,
    completion: @escaping ((any Error)?) -> Void
)
```

``` source
func reportNewIncomingCall(
    with UUID: UUID,
    update: CXCallUpdate
) async throws
```

## Parameters 

`UUID`  

The unique identifier of the call.

`update`  

The information for the call.

`completion`  

A block to be executed once the call is allowed or disallowed by the system. The block is executed on the delegate queue set by the setDelegate(_:queue:) method, or on a private serial queue if none is specified.

error  
If an error occurred, an error object indicating that the call was disallowed by the system, otherwise `nil`.

## Mentioned in 

Making and receiving VoIP calls

Sending End-to-End Encrypted VoIP Calls

## Discussion

Important

You can call this method from synchronous code using a completion handler, as shown on this page, or you can call it as an asynchronous method that has the following declaration:

```
func reportNewIncomingCall(with UUID: UUID, update: CXCallUpdate) async throws
```

For information about concurrency and asynchronous code in Swift, see Calling Objective-C APIs Asynchronously.

An incoming call may be disallowed by the system if, for example, the caller handle is blocked, or the user has Do Not Disturb enabled.

## See Also

### Reporting Calls

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

func reportCall(with: UUID, endedAt: Date?, reason: CXCallEndedReason)

Reports to the provider that a call with the specified identifier ended at a given date for a particular reason.

