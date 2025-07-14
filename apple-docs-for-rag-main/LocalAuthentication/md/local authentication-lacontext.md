

- Local Authentication
-  LAContext 

Class

# LAContext

A mechanism for evaluating authentication policies and access controls.

iOS 8.0+iPadOS 8.0+Mac Catalyst 13.1+macOS 10.10+visionOS 1.0+watchOS 3.0+

``` source
class LAContext
```

## Overview

You use an authentication context to evaluate the user’s identity, either with biometrics like Touch ID or Face ID, or by supplying the device passcode. The context handles user interaction, and also interfaces to the Secure Enclave, the underlying hardware element that manages biometric data. You create and configure the context, and ask it to carry out the authentication. You then receive an asynchronous callback, which provides an indication of authentication success or failure, and an error instance that explains the reason for a failure, if any.

Important

Include the NSFaceIDUsageDescription key in your app’s `Info.plist` file if your app allows biometric authentication. Otherwise, authorization requests may fail.

## Topics

### Checking availability

func canEvaluatePolicy(LAPolicy, error: NSErrorPointer) -> Bool

Assesses whether authentication can proceed for a given policy.

enum LAPolicy

The set of available local authentication policies.

var biometryType: LABiometryType

The type of biometric authentication supported by the device.

enum LABiometryType

The set of available biometric authentication types.

### Evaluating authentication policies

func evaluatePolicy(LAPolicy, localizedReason: String, reply: (Bool, (any Error)?) -> Void)

Evaluates the specified policy.

var evaluatedPolicyDomainState: Data?

The current state of the evaluated policy domain.

Deprecated

var maxBiometryFailures: NSNumber?

The number of biometric authentication failures after which the context falls back to another mechanism.

Deprecated

### Evaluating access controls

func evaluateAccessControl(SecAccessControl, operation: LAAccessControlOperation, localizedReason: String, reply: (Bool, (any Error)?) -> Void)

Evaluates an access control for a given operation.

enum LAAccessControlOperation

Operations to be evaluated for access control.

var interactionNotAllowed: Bool

A Boolean value indicating whether authentication can be interactive.

### Customizing authentication prompts

var localizedReason: String

The localized explanation for authentication shown in the dialog presented to the user.

var localizedFallbackTitle: String?

The localized title for the fallback button in the dialog presented to the user during authentication.

var localizedCancelTitle: String?

The localized title for the cancel button in the dialog presented to the user during authentication.

### Reusing device unlock state

var touchIDAuthenticationAllowableReuseDuration: TimeInterval

The duration for which Touch ID authentication reuse is allowable.

let LATouchIDAuthenticationMaximumAllowableReuseDuration: TimeInterval

The maximum allowable reuse duration.

### Managing credentials

func setCredential(Data?, type: LACredentialType) -> Bool

Sets an application-provided credential to be used when evaluating authentication.

func isCredentialSet(LACredentialType) -> Bool

Returns a Boolean value indicating whether the specified credential type is set.

enum LACredentialType

The types of credentials to be used for authentication.

### Invalidating the authentication context

func invalidate()

Invalidates the authentication context.

### Instance Properties

var domainState: LADomainState

Contains authentication domain state.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- Copyable
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol
- Observable
- ObservableObject

## See Also

### Authentication and access

class LARight

A grouped set of requirements that gate access to a resource or operation.

enum State

The possible states for a right during authorization.

