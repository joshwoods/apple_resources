

- Push to Talk
- PTInstantiationError
-  missingPushServerEnvironment 

Type Property

# missingPushServerEnvironment

An instantiation error that indicates the app doesn’t have the push notification capability in an enabled state.

iOS 16.0+iPadOS 16.0+Mac Catalyst 16.0+

``` source
static var missingPushServerEnvironment: PTInstantiationError.Code { get }
```

## See Also

### Constants

static var unknown: PTInstantiationError.Code

An instantiation error that indicates an unknown error.

static var invalidPlatform: PTInstantiationError.Code

An instantiation error that indicates the API isn’t available on the simulator or macOS devices.

static var missingBackgroundMode: PTInstantiationError.Code

An instantiation error that indicates the app doesn’t have the background mode in an enabled state.

static var missingEntitlement: PTInstantiationError.Code

An instantiation error that indicates the app is missing the entitlement.

static var instantiationAlreadyInProgress: PTInstantiationError.Code

An instantiation error that indicates there’s already an in-flight instantiation request.

