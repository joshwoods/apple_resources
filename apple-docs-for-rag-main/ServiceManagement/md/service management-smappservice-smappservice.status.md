

- Service Management
- SMAppService
-  SMAppService.Status 

Enumeration

# SMAppService.Status

Constants that describe the registration or authorization status of a helper executable.

Mac Catalyst 13.0+macOS 10.6+

``` source
enum Status
```

## Mentioned in 

Updating helper executables from earlier versions of macOS

## Topics

### Constants

case notRegistered

The service hasn’t registered with the Service Management framework, or the service attempted to reregister after it was already registered.

case enabled

The service has been successfully registered and is eligible to run.

case requiresApproval

The service has been successfully registered, but the user needs to take action in System Preferences.

case notFound

An error occurred and the framework couldn’t find this service.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

