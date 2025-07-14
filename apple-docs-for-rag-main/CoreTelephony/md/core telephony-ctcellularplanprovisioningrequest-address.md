

- Core Telephony
- CTCellularPlanProvisioningRequest
-  address 

Instance Property

# address

The address of the carrier network’s eSIM server.

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var address: String { get set }
```

## Discussion

The destination server must support the SMDP+ standard.

You must set this property for the request to be valid.

## See Also

### Specifying Request Properties

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

