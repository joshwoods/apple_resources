

- AppKit
-  NSRegisterServicesProvider(\_:\_:) 

Function

# NSRegisterServicesProvider(\_:\_:)

Registers a service provider.

macOS

``` source
func NSRegisterServicesProvider(
    _ provider: Any?,
    _ name: NSServiceProviderName
)
```

## Parameters 

`provider`  

The object providing the service you want to register.

`name`  

The unique name to associate with the service. This string is used to advertise the service to interested clients.

## Discussion

Use this function to register custom services not directly related to your application.

You should not use this function to register the services provided by your application. For your application’s services, you should use the servicesProvider method of NSApplication, passing a non-`nil` argument.

## See Also

### Registering Services

func NSUnregisterServicesProvider(NSServiceProviderName)

Unregisters a service provider.

func NSUpdateDynamicServices()

Causes the services information for the system to be updated.

typealias NSServiceProviderName

