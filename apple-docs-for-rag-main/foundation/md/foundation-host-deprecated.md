

- Foundation
-  Host Deprecated

Class

# Host

A representation of an individual host on the network.

macOS 10.0–15.4Deprecated

``` source
class Host
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Overview

The Host class provides methods to access the network name and address information for a host. Instances of the Host class represent individual *hosts* on a network. Use Host objects to get the current host’s names and addresses and to look up other hosts by name or by address.

To create an Host object, use the current(), init(address:), or init(name:) class methods (don’t use `alloc` and `init`). These methods use available network administration services to discover all names and addresses for the host requested. They don’t attempt to contact the host itself, however. This approach avoids untimely delays due to a host being unavailable, but it may result in incomplete information about the host.

An Host object contains all of the network addresses and names discovered for a given host by the network administration services. Each Host object may contain several addresses and have more than one name. If an Host object has more than one name, the additional names are variations on the same name, typically the basic host name plus the fully qualified domain name. For example, with a host name `"sales"` in the domain `"anycorp.com"`, an Host object can hold both the names `"sales"` and `"sales.anycorp.com"`.

Host methods are thread-safe.

## Topics

### Creating Hosts

class func current() -> Self

Returns an `NSHost` object representing the host the process is running on.

convenience init(address: String)

Returns the `NSHost` with the Internet address `address`.

convenience init(name: String?)

Returns a host with a specific name.

### Getting Host Information

var address: String?

Returns one of the network addresses of the receiver.

var addresses: [String]

Returns all the network addresses of the receiver.

var name: String?

Returns one of the hostnames of the receiver.

var localizedName: String?

Returns the name used as by default when publishing `NSNetServices`.

var names: [String]

Returns all the hostnames of the receiver.

### Comparing Hosts

func isEqual(to: Host) -> Bool

Indicates whether the receiver represents the same host as another `NSHost` object.

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSObjectProtocol

## See Also

### Sockets

class Port

An abstract class that represents a communication channel.

class SocketPort

A port that represents a BSD socket.

