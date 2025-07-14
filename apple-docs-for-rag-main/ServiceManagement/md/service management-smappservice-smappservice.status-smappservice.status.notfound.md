

- Service Management
- SMAppService
- SMAppService.Status
-  SMAppService.Status.notFound 

Case

# SMAppService.Status.notFound

An error occurred and the framework couldn’t find this service.

Mac Catalyst 13.0+macOS 10.6+

``` source
case notFound
```

## See Also

### Constants

case notRegistered

The service hasn’t registered with the Service Management framework, or the service attempted to reregister after it was already registered.

case enabled

The service has been successfully registered and is eligible to run.

case requiresApproval

The service has been successfully registered, but the user needs to take action in System Preferences.

