

- System Configuration
-  SCNetworkSetCopyServices(\_:) 

Function

# SCNetworkSetCopyServices(\_:)

Returns all network services associated with the specified set.

macOS 10.4+

``` source
func SCNetworkSetCopyServices(_ set: SCNetworkSet) -> CFArray?
```

## Parameters 

`set`  

The set (the complete configuration for a single location).

## Return Value

The list of network services associated with the set. You must release the returned value.

## See Also

### Configuring Network Sets

func SCNetworkSetAddService(SCNetworkSet, SCNetworkService) -> Bool

Adds the specified network service to the specified set.

func SCNetworkSetContainsInterface(SCNetworkSet, SCNetworkInterface) -> Bool

Returns a Boolean value indicating whether the specified interface is represented by at least one network service in the specified set.

func SCNetworkSetCopy(SCPreferences, CFString) -> SCNetworkSet?

Returns the set with the specified identifier.

func SCNetworkSetCopyAll(SCPreferences) -> CFArray?

Returns all available sets for the specified preferences session.

func SCNetworkSetCopyCurrent(SCPreferences) -> SCNetworkSet?

Returns the current set.

func SCNetworkSetCreate(SCPreferences) -> SCNetworkSet?

Creates a new set in the configuration.

func SCNetworkSetGetName(SCNetworkSet) -> CFString?

Returns the user-specified name associated with the specified set.

func SCNetworkSetGetServiceOrder(SCNetworkSet) -> CFArray?

Returns the user-specified ordering of network services within the specified set.

func SCNetworkSetGetSetID(SCNetworkSet) -> CFString?

Returns the identifier for the specified set.

func SCNetworkSetGetTypeID() -> CFTypeID

Returns the type identifier of all `SCNetworkSet` instances.

func SCNetworkSetRemove(SCNetworkSet) -> Bool

Removes the specified set from the configuration.

func SCNetworkSetRemoveService(SCNetworkSet, SCNetworkService) -> Bool

Removes the specified network service from the specified set.

func SCNetworkSetSetCurrent(SCNetworkSet) -> Bool

Specifies the set that should be the current set.

func SCNetworkSetSetName(SCNetworkSet, CFString?) -> Bool

Stores the user-specified name for the specified set.

func SCNetworkSetSetServiceOrder(SCNetworkSet, CFArray) -> Bool

Stores the user-specified ordering of network services for the specified set.

