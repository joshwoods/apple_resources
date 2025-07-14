

- Foundation
- Host
-  isEqual(to:) Deprecated

Instance Method

# isEqual(to:)

Indicates whether the receiver represents the same host as another `NSHost` object.

macOS 10.0–15.4Deprecated

``` source
func isEqual(to aHost: Host) -> Bool
```

Deprecated

Use Network framework instead, see deprecation notice in \

## Parameters 

`aHost`  

Host to compare the receiver to.

## Return Value

true when the receiver and `host` share at least one network address; false otherwise.

## See Also

### Related Documentation

var addresses: [String]

Returns all the network addresses of the receiver.

Deprecated

