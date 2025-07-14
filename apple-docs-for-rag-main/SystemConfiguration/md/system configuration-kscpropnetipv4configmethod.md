

- System Configuration
-  kSCPropNetIPv4ConfigMethod 

Global Variable

# kSCPropNetIPv4ConfigMethod

The IPv4 key `ConfigMethod`, whose value is of type `CFString`.

macOS 10.1+

``` source
let kSCPropNetIPv4ConfigMethod: CFString
```

## Discussion

This key can be passed the following constants:

- `kSCValNetIPv4ConfigMethodBOOTP`, which has the value `BOOTP`

- `kSCValNetIPv4ConfigMethodDHCP`, which has the value `DHCP`

- `kSCValNetIPv4ConfigMethodINFORM`, which has the value `INFORM`

- `kSCValNetIPv4ConfigMethodLinkLocal`, which has the value `LinkLocal`

- `kSCValNetIPv4ConfigMethodManual`, which has the value `Manual`

- `kSCValNetIPv4ConfigMethodPPP`, which has the value `PPP`

## See Also

### Constants

let kSCPropNetIPv4Addresses: CFString

The IPv4 key `Addresses`, whose value is of type `CFArray`, containing elements of type `CFString`.

let kSCPropNetIPv4DHCPClientID: CFString

The IPv4 key `DHCPClientID`, whose value is of type `CFString`.

let kSCPropNetIPv4Router: CFString

The IPv4 key `Router`, whose value is of type `CFString`.

let kSCPropNetIPv4SubnetMasks: CFString

The IPv4 key `SubnetMasks`, whose value is of type `CFArray`, containing elements of type `CFString`.

let kSCPropNetIPv4DestAddresses: CFString

The IPv4 key `DestAddresses`, whose value is of type `CFArray`, containing elements of type `CFString`.

let kSCPropNetIPv4BroadcastAddresses: CFString

The IPv4 key `BroadcastAddresses`, whose value is of type `CFArray`, containing elements of type `CFString`.

