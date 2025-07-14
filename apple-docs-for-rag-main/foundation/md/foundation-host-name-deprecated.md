

- Foundation
- Host
-  name Deprecated

Instance Property

# name

Returns one of the hostnames of the receiver.

macOS 10.0–15.4Deprecated

``` source
var name: String? { get }
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Return Value

One of the hostnames of the receiver. Can be either a simple hostname, such as `"sales"`, or a fully qualified domain name, such as `"sales.anycorp.com"`.

## See Also

### Getting Host Information

var address: String?

Returns one of the network addresses of the receiver.

Deprecated

var addresses: [String]

Returns all the network addresses of the receiver.

Deprecated

var localizedName: String?

Returns the name used as by default when publishing `NSNetServices`.

Deprecated

var names: [String]

Returns all the hostnames of the receiver.

Deprecated

