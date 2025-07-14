

- AudioDriverKit
- IOUserAudioDriver
-  NewUserClient 

Instance Method

# NewUserClient

Requests the creation of a new user client for the service.

DriverKit 21.0+

``` source
kern_return_t NewUserClient(uint32_t in_type, IOUserClient * * out_user_client);
```

## Parameters 

`in_type`  

The type passed to IOServiceOpen(_:_:_:_:).

`out_user_client`  

A pointer to a variable for returning the new user client object. Upon the successful creation of the user client object, assign it to this variable.

## Return Value

kIOReturnSuccess on success, or another value if an error occurs. For a list of error codes, see Error Codes.

## Discussion

Override this method if your service supports communication though an external user client. When an app calls IOServiceOpen(_:_:_:_:) to start a new service, the system calls this method on the service passed to that function. In your implementation, call the Create method to create a new IOUserClient object for your service and return that object in the `userClient` parameter.

