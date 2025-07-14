

- Core Telephony
-  CTCellularPlanProvisioningRequest 

Class

# CTCellularPlanProvisioningRequest

A request specifying an eSIM to download and install.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
class CTCellularPlanProvisioningRequest
```

## Overview

You must set the address property for the request to be valid. All other properties are optional.

This class is only available to carrier apps with suitable entitlements.

## Topics

### Specifying Request Properties

var address: String

The address of the carrier network’s eSIM server.

var confirmationCode: String?

The provisioning request’s confirmation code, provided by the network operator when initiating an eSIM download.

var eid: String?

The provisioning request’s eUICC identifier (EID).

var iccid: String?

The provisioning request’s Integrated Circuit Card Identifier (ICCID).

var matchingID: String?

The provisioning request’s matching identifier (MatchingID).

var oid: String?

The provisioning request’s Object Identifier (OID).

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### eSIM

class CTCellularPlanProvisioning

An object you use to download and install a carrier eSIM.

