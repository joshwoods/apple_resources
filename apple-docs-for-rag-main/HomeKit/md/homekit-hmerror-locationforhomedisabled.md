

- HomeKit
- HMError
-  locationForHomeDisabled 

Type Property

# locationForHomeDisabled

An error indicating the home’s location is disabled.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var locationForHomeDisabled: HMError.Code { get }
```

## See Also

### Detecting authorization errors

static var invalidOrMissingAuthorizationData: HMError.Code

An error indicating the authorization data is invalid or missing.

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

static var ownershipFailure: HMError.Code

The ownership code did not match.

static var securityFailure: HMError.Code

A security failure.

