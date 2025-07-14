

- DriverKit
-  IOUserServer 

Class

# IOUserServer

A system-managed service.

DriverKitiOSiPadOSmacOS

``` source
class IOUserServer;
```

## Overview

You do not create or use instances of this class directly. The system creates them to manage individual services.

## Topics

### Configuring the User Server

Create

init

free

### Managing the Server Lifecycle

LoadModule

Exit

### Instance Methods

RegisterService

## Relationships

### Inherits From

- IOService

## See Also

### External drivers

IOUserClient

A connection to another service that the system manages.

com.apple.developer.driverkit.userclient-access

An array of strings that represent macOS driver extensions that may communicate with other DriverKit services.

Communicating between a DriverKit extension and a client app

Send and receive different kinds of data securely by validating inputs and asynchronously by storing and using a callback.

