

- DriverKit
- IOStateReporter_IVars
-  handleSetStateByIndices 

Instance Method

# handleSetStateByIndices

DriverKitiOSiPadOSmacOS

``` source
IOReturn handleSetStateByIndices(int channel_index, int new_state_index, uint64_t last_intransition, uint64_t prev_state_residency);
```

## Parameters 

`channel_index`  

- 0.., available from getChannelIndex()

`new_state_index`  

- New state for the channel

`last_intransition`  

- to remove: time of most recent entry

`prev_state_residency`  

- to remove: time spent in previous state

## Return Value

Appropriate IOReturn code

## Discussion

Locked version of IOReporter::setStateByIndices(). This method may be overriden by sub-classes.

Locking: Caller must ensure that the reporter (data) lock is held.

