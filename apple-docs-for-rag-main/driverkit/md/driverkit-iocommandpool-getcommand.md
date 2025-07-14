

- DriverKit
- IOCommandPool
-  getCommand 

Instance Method

# getCommand

DriverKitiOSiPadOSmacOS

``` source
IOCommandPtr getCommand(bool blockForCommand);
```

## Parameters 

`blockForCommand`  

If the caller would like to have its thread slept until a command is available, it should pass true, else false.

## Return Value

If the caller passes true in blockForCommand, getCommand guarantees that the result will be a pointer to an IOCommand object from the pool. If the caller passes false, s/he is responsible for checking whether a non-NULL pointer was returned.

## Discussion

The getCommand method is used to get a pointer to an object of type IOCommand from the pool.

