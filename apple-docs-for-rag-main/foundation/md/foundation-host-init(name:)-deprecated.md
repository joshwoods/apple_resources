

- Foundation
- Host
-  init(name:) Deprecated

Initializer

# init(name:)

Returns a host with a specific name.

macOS 10.0–15.4Deprecated

``` source
convenience init(name: String?)
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Parameters 

`name`  

Name of the host to look up. Can be either a simple hostname, such as `"sales"`, or a fully qualified domain name, such as `"sales.anycorp.com"`.

## Return Value

The host named `hostname`.

## See Also

### Creating Hosts

class func current() -> Self

Returns an `NSHost` object representing the host the process is running on.

Deprecated

convenience init(address: String)

Returns the `NSHost` with the Internet address `address`.

Deprecated

