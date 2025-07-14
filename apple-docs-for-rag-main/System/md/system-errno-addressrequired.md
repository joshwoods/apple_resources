

- System
- Errno
-  addressRequired 

Type Property

# addressRequired

Destination address required.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var addressRequired: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

A required address was omitted from a socket operation.

The corresponding C error is `EDESTADDRREQ`.

## See Also

### Network Address Errors

static var addressFamilyNotSupported: Errno

The address family isn’t supported by the protocol family.

static var addressInUse: Errno

Address already in use.

static var addressNotAvailable: Errno

Can’t assign the requested address.

