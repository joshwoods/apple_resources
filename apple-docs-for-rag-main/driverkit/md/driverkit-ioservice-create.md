

- DriverKit
- IOService
-  Create 

Instance Method

# Create

Requests the creation of a new service object.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t Create(IOService * provider, const IOPropertyName propertiesKey, IOService * * result);
```

## Parameters 

`provider`  

The provider to associate with the new service object. Always specify the current service object as the provider.

`propertiesKey`  

The name of a property associated with the current service. The value of this property must be an OSDictionary object, and the dictionary should contain the kIOClassKey, kIOUserClassKey, and kIOServiceDEXTEntitlementsKey matching keys.

`result`  

The service object for the newly created service. The class of this object is the one you specified using the kIOClassKey in the `propertiesKey` dictionary This method retains the object, and you are responsible for releasing it.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Call this method from your NewUserClient method when the system asks you to create a new service. The keys in the `propertiesKey` dictionary describe the new service. Use the kIOUserClassKey key to specify the name of the custom IOService subclass that you want the system to instantiate. Use the kIOClassKey to specify the name of the custom IOUserClient subclass to return to clients of your service. Use the kIOServiceDEXTEntitlementsKey key to specify an array of entitlement strings to match against the process of the new service. The new service must contain all of the requested entitlements.

## See Also

### Creating a New Service

NewUserClient

Requests the creation of a new user client for the service.

