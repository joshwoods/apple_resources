

- Service Management
-  kSMErrorAuthorizationFailure 

Global Variable

# kSMErrorAuthorizationFailure

The authorization requested failed.

Mac Catalyst 13.0+macOS 10.6+

``` source
var kSMErrorAuthorizationFailure: Int { get }
```

## Discussion

The request requires authorization (such as, adding a job to the kSMDomainSystemLaunchd), but the `AuthorizationRef` doesn’t contain the required right.

## See Also

### Constants

var kSMErrorAlreadyRegistered: Int

The application is already registered.

var kSMErrorInternalFailure: Int

An internal failure has occurred.

var kSMErrorInvalidPlist: Int

The app’s property list is invalid.

var kSMErrorInvalidSignature: Int

The app’s code signature doesn’t meet the requirements to perform the operation.

var kSMErrorJobMustBeEnabled: Int

var kSMErrorJobNotFound: Int

The system can’t find the specified job.

var kSMErrorJobPlistNotFound: Int

var kSMErrorLaunchDeniedByUser: Int

The user denied the app’s launch request.

var kSMErrorServiceUnavailable: Int

The service necessary to perform this operation is unavailable or is no longer accepting requests.

var kSMErrorToolNotValid: Int

The specified path doesn’t exist or the helper tool at the specified path isn’t valid.

