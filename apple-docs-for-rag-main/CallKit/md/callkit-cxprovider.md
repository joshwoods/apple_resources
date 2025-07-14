

- CallKit
-  CXProvider 

Class

# CXProvider

An object that represents a telephony provider.

iOS 10.0+iPadOS 10.0+Mac Catalyst 10.0+visionOS 1.0+watchOS 9.0+

``` source
class CXProvider
```

## Mentioned in 

Making and receiving VoIP calls

## Overview

A CXProvider object is responsible for reporting out-of-band notifications that occur to the system. A VoIP app should create only one instance of CXProvider and store it for use globally. A CXProvider object is initialized with a CXProviderConfiguration object to specify the behavior and capabilities of calls. Each provider can specify an object conforming to the CXProviderDelegate protocol to respond to events, such as the call starting, the call being put on hold, or the provider’s audio session being activated.

### Subclassing Notes

CXProvider is not intended for subclassing.

## Topics

### Creating New Providers

init(configuration: CXProviderConfiguration)

Initializes a new provider with the specified configuration.

### Setting the Delegate

func setDelegate((any CXProviderDelegate)?, queue: dispatch_queue_t?)

Sets a provider delegate, specifying an optional queue on which to execute delegate methods.

### Accessing Provider Attributes

var configuration: CXProviderConfiguration

The configuration of the provider.

### Accessing Pending Transaction and Call Actions

var pendingTransactions: [CXTransaction]

Incomplete transactions.

func pendingCallActions(of: AnyClass, withCall: UUID) -> [CXCallAction]

Returns all call actions in any pending transactions of the specified class for the specified call identifier that are incomplete.

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

func reportCall(with: UUID, endedAt: Date?, reason: CXCallEndedReason)

Reports to the provider that a call with the specified identifier ended at a given date for a particular reason.

### Invalidating a Provider

func invalidate()

Invalidates the provider and completes all active calls with an error.

### Handling Errors

enum CXCallEndedReason

The reason that a call ended.

struct CXError

Error codes for the CallKit errors.

enum Code

Error codes for the CallKit errors.

struct CXErrorCodeIncomingCallError

Codes for errors that occur during incoming calls.

enum Code

Codes for errors that occur during incoming calls.

struct CXErrorCodeNotificationServiceExtensionError

Errors that can occur when reporting new, incoming VoIP calls.

let CXErrorDomain: String

The domain for CallKit errors.

let CXErrorDomainIncomingCall: String

The domain for errors that occur during incoming calls.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Essentials

protocol CXProviderDelegate

A collection of methods that a telephony provider object calls.

class CXProviderConfiguration

An encapsulation of the configuration of a provider object.

Making and receiving VoIP calls

Initiate outgoing calls with VoIP and configure your app to receive incoming calls.

VoIP calling with CallKit

Use the CallKit framework to integrate native VoIP calling.

Preparing your app to be the default calling app

Configure your CallKit or LiveCommunicationKit app so people can set it as the default calling app on their device.

