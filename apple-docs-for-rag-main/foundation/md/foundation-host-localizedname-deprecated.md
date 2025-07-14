

- Foundation
- Host
-  localizedName Deprecated

Instance Property

# localizedName

Returns the name used as by default when publishing `NSNetServices`.

macOS 10.6–15.4Deprecated

``` source
var localizedName: String? { get }
```

## Return Value

A string containing the computer name.

## Discussion

This is the name displayed in the Finder sidebar, as well as in the Sharing preference panel.

This method only returns an `NSString` when sent to the current() instance, all other instances currently return `nil`.

This property is key-value observable.

## See Also

### Getting Host Information

var address: String?

Returns one of the network addresses of the receiver.

Deprecated

var addresses: [String]

Returns all the network addresses of the receiver.

Deprecated

var name: String?

Returns one of the hostnames of the receiver.

Deprecated

var names: [String]

Returns all the hostnames of the receiver.

Deprecated

