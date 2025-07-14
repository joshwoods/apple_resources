

- DriverKit
-  IOUserClient 

Class

# IOUserClient

A connection to another service that the system manages.

DriverKitiOSiPadOSmacOS

``` source
class IOUserClient;
```

## Overview

An application may open an IOUserClient by calling IOServiceOpen(). This results in a call to the IOService::NewUserClient API to create an instance representing the connection. and to receive untyped data via IOConnectMethod/IOConnectAsyncMethod. As an IOService subclass, IOUserClient receives the normal Start()/Stop() lifecyle calls.

## Topics

### Configuring a User Client

init

free

### Communicating with the Client

AsyncCompletion

Send asynchronous arguments to a completion supplied by ExternalMethod().

KernelCompletion

IOUserClientAsyncArgumentsArray

Arguments Array Maximum

IOUserClientAsyncReferenceArray

Reference Array Maximum

### Responding to Messages

ExternalMethod

Receive arguments from IOKit.framework IOConnectMethod calls.

IOUserClientMethodArguments

Arguments to pass to IOConnectMethod calls.

IOUserClientMethodDispatch

A structure that specifies how to validate the arguments passed to a client method function.

IOUserClientMethodFunction

### Mapping to the Client’s Memory Space

CopyClientMemoryForType

Return an IOMemoryDescriptor to be mapped into the client task.

Copy Client Memory Options

### Instance Methods

CopyClientEntitlements

CreateMemoryDescriptorFromClient

## Relationships

### Inherits From

- IOService

## See Also

### External drivers

IOUserServer

A system-managed service.

com.apple.developer.driverkit.userclient-access

An array of strings that represent macOS driver extensions that may communicate with other DriverKit services.

Communicating between a DriverKit extension and a client app

Send and receive different kinds of data securely by validating inputs and asynchronously by storing and using a callback.

