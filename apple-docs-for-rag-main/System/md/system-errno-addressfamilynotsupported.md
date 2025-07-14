

- System
- Errno
-  addressFamilyNotSupported 

Type Property

# addressFamilyNotSupported

The address family isn’t supported by the protocol family.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var addressFamilyNotSupported: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

An address incompatible with the requested protocol was used. For example, you shouldn’t necessarily expect to be able to use name server addresses with ARPA Internet protocols.

The corresponding C error is `EAFNOSUPPORT`.

## See Also

### Network Address Errors

static var addressInUse: Errno

Address already in use.

static var addressNotAvailable: Errno

Can’t assign the requested address.

static var addressRequired: Errno

Destination address required.

