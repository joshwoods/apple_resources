

- System Configuration
-  kSCPropNetIPv6ConfigMethod 

Global Variable

# kSCPropNetIPv6ConfigMethod

The IPv6 key `ConfigMethod`, whose value is of type `CFString`.

macOS 10.1+

``` source
let kSCPropNetIPv6ConfigMethod: CFString
```

## Discussion

This key can be passed the following constants:

- `kSCValNetIPv6ConfigMethodAutomatic`, which has the value `Automatic`

- `kSCValNetIPv6ConfigMethodManual`, which has the value `Manual`

- `kSCValNetIPv6ConfigMethodRouterAdvertisement`, which has the value `RouterAdvertisement`

- `kSCValNetIPv6ConfigMethod6to4`, which has the value `6to4`

## See Also

### Constants

let kSCPropNetIPv6Addresses: CFString

The IPv6 key `Addresses`, whose value is of type `CFArray`, containing elements of type `CFString`.

let kSCPropNetIPv6DestAddresses: CFString

The IPv6 key `DestAddresses`, whose value is of type `CFArray`, containing elements of type `CFString`.

let kSCPropNetIPv6Flags: CFString

The IPv6 key `Flags`, whose value is of type `CFNumber`.

let kSCPropNetIPv6PrefixLength: CFString

The IPv6 key `PrefixLength`, whose value is of type `CFArray`, containing elements of type `CFNumber`.

let kSCPropNetIPv6Router: CFString

The IPv6 key `Router`, whose value is of type `CFString`.

