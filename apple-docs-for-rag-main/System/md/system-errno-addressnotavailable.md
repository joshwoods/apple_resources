

- System
- Errno
-  addressNotAvailable 

Type Property

# addressNotAvailable

Can’t assign the requested address.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var addressNotAvailable: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

This error normally results from an attempt to create a socket with an address that isn’t on this machine.

The corresponding C error is `EADDRNOTAVAIL`.

## See Also

### Network Address Errors

static var addressFamilyNotSupported: Errno

The address family isn’t supported by the protocol family.

static var addressInUse: Errno

Address already in use.

static var addressRequired: Errno

Destination address required.

