

- Service Management
- SMAppService
- SMAppService.Status
-  SMAppService.Status.notRegistered 

Case

# SMAppService.Status.notRegistered

The service hasn’t registered with the Service Management framework, or the service attempted to reregister after it was already registered.

Mac Catalyst 13.0+macOS 10.6+

``` source
case notRegistered
```

## See Also

### Constants

case enabled

The service has been successfully registered and is eligible to run.

case requiresApproval

The service has been successfully registered, but the user needs to take action in System Preferences.

case notFound

An error occurred and the framework couldn’t find this service.

