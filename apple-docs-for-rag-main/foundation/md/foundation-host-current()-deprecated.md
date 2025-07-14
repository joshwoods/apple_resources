

- Foundation
- Host
-  current() Deprecated

Type Method

# current()

Returns an `NSHost` object representing the host the process is running on.

macOS 10.0–15.4Deprecated

``` source
class func current() -> Self
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Return Value

`NSHost` object for the process’s host.

## Discussion

This method executes synchronously. The execution time of this method can be highly variable, depending on the local network configuration, and may block for several seconds if the network is unreachable. To avoid blocking execution on the main thread, you should call this method in an Operation or *Grand Central Dispatch* block that executes asynchronously in the background.

## See Also

### Creating Hosts

convenience init(address: String)

Returns the `NSHost` with the Internet address `address`.

Deprecated

convenience init(name: String?)

Returns a host with a specific name.

Deprecated

