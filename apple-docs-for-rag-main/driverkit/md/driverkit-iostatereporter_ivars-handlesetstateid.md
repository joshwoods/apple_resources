

- DriverKit
- IOStateReporter_IVars
-  handleSetStateID 

Instance Method

# handleSetStateID

DriverKitiOSiPadOSmacOS

``` source
IOReturn handleSetStateID(uint64_t channel_id, int state_index, uint64_t state_id);
```

## Parameters 

`channel_id`  

- ID of channel containing the state in question

`state_index`  

- index of state to give an ID: \[0..(nstates-1)\]

`state_id`  

- 64-bit state ID, for ASCII, use IOREPORT_MAKEID

## Return Value

Appropriate IOReturn code

## Discussion

Locked version of IOReporter::setStateID(). This method may be overriden by sub-classes

Locking: Caller must ensure that the reporter (data) lock is held.

