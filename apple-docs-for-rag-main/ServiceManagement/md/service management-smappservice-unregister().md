

- Service Management
- SMAppService
-  unregister() 

Instance Method

# unregister()

Unregisters the service so the system no longer launches it.

Mac Catalyst 16.0+macOS 13.0+

``` source
func unregister() throws
```

## Discussion

This is the opposite operation of register().

If the service corresponds to a LoginItem, LaunchAgent, or LaunchDaemon and the service is currently running it, the system terminates it. If the service corresponds to the main application, it continues running, but becomes unregistered to prevent future launches at login.

If the service is already unregistered, this method returns kSMErrorJobNotFound.

## See Also

### Registering services

func register() throws

Registers the service so it can begin launching subject to user approval.

func unregister(completionHandler: ((any Error)?) -> Void)

Unregisters the service so the system no longer launches it and calls a completion handler you provide with the resulting error value.

