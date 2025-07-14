

- Service Management
- SMAppService
- SMAppService.Status
-  SMAppService.Status.enabled 

Case

# SMAppService.Status.enabled

The service has been successfully registered and is eligible to run.

Mac Catalyst 13.0+macOS 10.6+

``` source
case enabled
```

## See Also

### Constants

case notRegistered

The service hasn’t registered with the Service Management framework, or the service attempted to reregister after it was already registered.

case requiresApproval

The service has been successfully registered, but the user needs to take action in System Preferences.

case notFound

An error occurred and the framework couldn’t find this service.

