

- Foundation
- Host
-  init(address:) Deprecated

Initializer

# init(address:)

Returns the `NSHost` with the Internet address `address`.

macOS 10.0–15.4Deprecated

``` source
convenience init(address: String)
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Parameters 

`address`  

Network address to look up. For example, `"127.0.0.1"` or `"fe80::1"`.

## Return Value

The host for `address`.

## See Also

### Creating Hosts

class func current() -> Self

Returns an `NSHost` object representing the host the process is running on.

Deprecated

convenience init(name: String?)

Returns a host with a specific name.

Deprecated

