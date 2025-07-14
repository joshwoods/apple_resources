

- Core Telephony
- CTCellularPlanProvisioningRequest
-  matchingID 

Instance Property

# matchingID

The provisioning request’s matching identifier (MatchingID).

iOS 12.0+iPadOS 12.0+Mac Catalyst 13.1+

``` source
var matchingID: String? { get set }
```

## Discussion

See GSMA SGP.22 for description. This property is optional.

## See Also

### Specifying Request Properties

var address: String

The address of the carrier network’s eSIM server.

var confirmationCode: String?

The provisioning request’s confirmation code, provided by the network operator when initiating an eSIM download.

var eid: String?

The provisioning request’s eUICC identifier (EID).

var iccid: String?

The provisioning request’s Integrated Circuit Card Identifier (ICCID).

var oid: String?

The provisioning request’s Object Identifier (OID).

