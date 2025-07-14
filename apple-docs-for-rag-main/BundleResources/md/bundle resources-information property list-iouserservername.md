

- Bundle Resources
- Information Property List
-  IOUserServerName 

Property List Key

# IOUserServerName

The name that the system uses to facilitate communication between your driver and other clients.

macOS 10.14+

## Details 

Type  

string

## Discussion

Typically, you set the value of this key to your kext or DriverKit extension’s bundle identifier. The system registers your driver under the specified server name, and uses that name to facilitate communications between your driver and other clients, including the kernel itself.

## See Also

### Driver Classes

IOUserClass

The name of your driver’s main class, which is the entry point for interacting with your driver’s code.

IOProviderClass

The name of the class that your driver expects to provide the implementation for its provider object.

IOClass

The name of the class to instantiate from your driver.

IOUserClientClass

The name of the class to instantiate when the system requires a client connection to the driver.

