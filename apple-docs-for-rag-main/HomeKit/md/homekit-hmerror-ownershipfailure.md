

- HomeKit
- HMError
-  ownershipFailure 

Type Property

# ownershipFailure

The ownership code did not match.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+tvOS 13.0+visionOS 1.0+watchOS 6.0+

``` source
static var ownershipFailure: HMError.Code { get }
```

## See Also

### Detecting authorization errors

static var invalidOrMissingAuthorizationData: HMError.Code

An error indicating the authorization data is invalid or missing.

static var locationForHomeDisabled: HMError.Code

An error indicating the home’s location is disabled.

static var homeAccessNotAuthorized: HMError.Code

An error indicating access to the home is not authorized.

static var insufficientPrivileges: HMError.Code

An error indicating insufficient privileges for the operation.

static var messageAuthenticationFailed: HMError.Code

A message authentication failure.

static var notAuthorizedForLocationServices: HMError.Code

An error indicating location services are not authorized.

static var notAuthorizedForMicrophoneAccess: HMError.Code

An error indicating microphone access is not authorized.

static var notSignedIntoiCloud: HMError.Code

An error indicating the user is not signed into iCloud.

static var securityFailure: HMError.Code

A security failure.

