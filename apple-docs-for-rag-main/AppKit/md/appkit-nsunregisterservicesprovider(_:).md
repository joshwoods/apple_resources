

- AppKit
-  NSUnregisterServicesProvider(\_:) 

Function

# NSUnregisterServicesProvider(\_:)

Unregisters a service provider.

macOS

``` source
func NSUnregisterServicesProvider(_ name: NSServiceProviderName)
```

## Parameters 

`name`  

The name of the service you want to unregister.

## Discussion

Use this function to unregister custom services not directly related to your application.

You should not use this function to unregister the services provided by your application. For your application’s services, you should use the servicesProvider method of NSApplication, passing a `nil` argument.

## See Also

### Registering Services

func NSRegisterServicesProvider(Any?, NSServiceProviderName)

Registers a service provider.

func NSUpdateDynamicServices()

Causes the services information for the system to be updated.

typealias NSServiceProviderName

