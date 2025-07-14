

- Bundle Resources
- Information Property List
-  IOUserClientClass 

Property List Key

# IOUserClientClass

The name of the class to instantiate when the system requires a client connection to the driver.

macOS 10.0+

## Details 

Type  

string

## Discussion

The value of this key is a string that contains the name of an IOService subclass in your driver.

## See Also

### Driver Classes

IOUserClass

The name of your driver’s main class, which is the entry point for interacting with your driver’s code.

IOProviderClass

The name of the class that your driver expects to provide the implementation for its provider object.

IOClass

The name of the class to instantiate from your driver.

IOUserServerName

The name that the system uses to facilitate communication between your driver and other clients.

