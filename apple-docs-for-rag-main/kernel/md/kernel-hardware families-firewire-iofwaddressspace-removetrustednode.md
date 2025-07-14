

- Kernel
- Hardware Families
- FireWire
- IOFWAddressSpace
-  removeTrustedNode 

# removeTrustedNode

Remove a trusted node.

``` source
inline void removeTrustedNode(
 IOFireWireDevice *device ) 
```

## Parameters 

`device`  

object pointing to a FireWire node on the bus.

## Return Value

none

## See Also

### Miscellaneous

activate

Address space is ready for handling requests.

addTrustedNode

Add a trusted node.

contains

returns number of bytes starting at addr in this space

deactivate

Address space request handler is disabled.

doLock

A method for processing a lock request.

doRead

An abstract method for processing an address space read request

doWrite

An abstract method for processing an address space write request

intersects

Checks this address space intersects with the given address range. Currently only supports IOFWPsuedoAddressSpaces.

isExclusive

Checks if an address space wants exclusive control of its address range

isTrustedNode

returns true if the node is added as a trusted node

removeAllTrustedNodes

Remove all trusted nodes.

setExclusive

Sets if this address space requires exclusive control of its address range. Exclusivity should be set before an address space is activated.

