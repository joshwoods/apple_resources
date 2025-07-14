

- Bundle Resources
- Information Property List
-  IOProviderClass 

Property List Key

# IOProviderClass

The name of the class that your driver expects to provide the implementation for its provider object.

macOS 10.0+

## Details 

Type  

string

## Discussion

The value of this key is a string that contains the name of an IOService subclass. This class corresponds to the provider object that the system passes to your IOService subclass at startup. (For a kernel extension, the system passes the provider object to the start method of your IOService subclass. For a DriverKit extension, the system passes it to the Start method of your IOService subclass.) Use the provider object in your driver you receive to communicate with the underlying device.

## See Also

### Driver Classes

IOUserClass

The name of your driver’s main class, which is the entry point for interacting with your driver’s code.

IOClass

The name of the class to instantiate from your driver.

IOUserClientClass

The name of the class to instantiate when the system requires a client connection to the driver.

IOUserServerName

The name that the system uses to facilitate communication between your driver and other clients.

