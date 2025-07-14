

- System
- Errno
-  addressInUse 

Type Property

# addressInUse

Address already in use.

iOS 14.0+iPadOS 14.0+Mac Catalyst 14.0+macOS 11.0+tvOS 14.0+visionOS 1.0+watchOS 7.0+

``` source
static var addressInUse: Errno { get }
```

## Mentioned in 

Adopting Swift Error Constants

## Discussion

Only one use of each address is normally permitted.

The corresponding C error is `EADDRINUSE`.

## See Also

### Network Address Errors

static var addressFamilyNotSupported: Errno

The address family isn’t supported by the protocol family.

static var addressNotAvailable: Errno

Can’t assign the requested address.

static var addressRequired: Errno

Destination address required.

