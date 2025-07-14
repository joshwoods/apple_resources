

- DriverKit
- IOService
-  NewUserClient 

Instance Method

# NewUserClient

Requests the creation of a new user client for the service.

DriverKitiOSiPadOSmacOS

``` source
kern_return_t NewUserClient(uint32_t type, IOUserClient * * userClient);
```

## Parameters 

`type`  

The type passed to IOServiceOpen(_:_:_:_:).

`userClient`  

A pointer to a variable for returning the new user client object. Upon the successful creation of the user client object, assign it to this variable.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Override this method if your service supports communication though an external user client. When an app calls IOServiceOpen(_:_:_:_:) to start a new service, the system calls this method on the service passed to that function. In your implementation, call the Create method to create a new IOUserClient object for your service and return that object in the `userClient` parameter.

## See Also

### Creating a New Service

Create

Requests the creation of a new service object.

