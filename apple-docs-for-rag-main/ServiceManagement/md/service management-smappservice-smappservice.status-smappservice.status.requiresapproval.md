

- Service Management
- SMAppService
- SMAppService.Status
-  SMAppService.Status.requiresApproval 

Case

# SMAppService.Status.requiresApproval

The service has been successfully registered, but the user needs to take action in System Preferences.

Mac Catalyst 13.0+macOS 10.6+

``` source
case requiresApproval
```

## Discussion

The Service Management framework successfully registered this service, but the user needs to take action in System Settings before the service is eligible to run. The framework also returns this status if the user revokes consent for the service to run in System Settings.

## See Also

### Constants

case notRegistered

The service hasn’t registered with the Service Management framework, or the service attempted to reregister after it was already registered.

case enabled

The service has been successfully registered and is eligible to run.

case notFound

An error occurred and the framework couldn’t find this service.

