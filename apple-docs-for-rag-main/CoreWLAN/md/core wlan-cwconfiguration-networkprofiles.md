

- Core WLAN
- CWConfiguration
-  networkProfiles 

Instance Property

# networkProfiles

An array of remembered CWNetworkProfile objects.

macOS 10.7+

``` source
@NSCopying
var networkProfiles: NSOrderedSet { get }
```

## Discussion

The order of this array corresponds to the order in which the the CWNetworkProfile objects participate in the auto-join process.

## See Also

### Instance Properties

var rememberJoinedNetworks: Bool

AirPort client will remember all joined networks.

var requireAdministratorForAssociation: Bool

Require an administrator password to change networks.

var requireAdministratorForIBSSMode: Bool

Require an administrator password to create a computer-to-computer network.

var requireAdministratorForPower: Bool

Require an administrator password to change the interface power state.

