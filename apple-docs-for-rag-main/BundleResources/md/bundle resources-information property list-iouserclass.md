

- Bundle Resources
- Information Property List
-  IOUserClass 

Property List Key

# IOUserClass

The name of your driver’s main class, which is the entry point for interacting with your driver’s code.

macOS 10.14+

## Details 

Type  

string

## Discussion

Include this key only in the personality dictionary of a DriverKit extension, and use it to specify the name of the custom IOService subclass that provides your driver’s behavior. When it’s time to load your driver, the system instantiates the specified class and begins the initialization and startup processes.

## See Also

### Driver Classes

IOProviderClass

The name of the class that your driver expects to provide the implementation for its provider object.

IOClass

The name of the class to instantiate from your driver.

IOUserClientClass

The name of the class to instantiate when the system requires a client connection to the driver.

IOUserServerName

The name that the system uses to facilitate communication between your driver and other clients.

