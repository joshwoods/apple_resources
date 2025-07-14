

- Bundle Resources
- Information Property List
-  IOClass 

Property List Key

# IOClass

The name of the class to instantiate from your driver.

macOS 10.0+

## Details 

Type  

string

## Discussion

The value of this key is a string that contains the name of a custom IOService subclass in your driver. When the system successfully matches one of your driver’s personalities to a device, it instantiates the class in this key and calls its start method.

For the personalities in a DriverKit extension, specify the value `IOUserService` unless otherwise directed by the documentation. For example, the IOUserHIDEventService class expects you to specify the value `AppleUserHIDEventService`.

## See Also

### Driver Classes

IOUserClass

The name of your driver’s main class, which is the entry point for interacting with your driver’s code.

IOProviderClass

The name of the class that your driver expects to provide the implementation for its provider object.

IOUserClientClass

The name of the class to instantiate when the system requires a client connection to the driver.

IOUserServerName

The name that the system uses to facilitate communication between your driver and other clients.

