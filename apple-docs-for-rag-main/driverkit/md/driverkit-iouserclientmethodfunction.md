

- DriverKit
-  IOUserClientMethodFunction 

Type Alias

# IOUserClientMethodFunction

DriverKitiOSiPadOSmacOS

``` source
typedef int (*)(class OSObject *, void *, struct IOUserClientMethodArguments *) IOUserClientMethodFunction;
```

## See Also

### Responding to Messages

ExternalMethod

Receive arguments from IOKit.framework IOConnectMethod calls.

IOUserClientMethodArguments

Arguments to pass to IOConnectMethod calls.

IOUserClientMethodDispatch

A structure that specifies how to validate the arguments passed to a client method function.

