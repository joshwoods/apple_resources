

- DriverKit
- IOStateReporter_IVars
-  handleOverrideChannelStateByIndices 

Instance Method

# handleOverrideChannelStateByIndices

DriverKitiOSiPadOSmacOS

``` source
IOReturn handleOverrideChannelStateByIndices(int channel_index, int state_index, uint64_t time_in_state, uint64_t intransitions, uint64_t last_intransition);
```

## Parameters 

`channel_index`  

- index of the channel which state is to be updated

`state_index`  

- index of the state id for the channel

`time_in_state`  

- time used as new total time in state

`intransitions`  

- total number of transitions into state

`last_intransition`  

- mach_absolute_time of most recent entry (opt)

## Return Value

Appropriate IOReturn code

## Discussion

Locked version of IOReporter::overrideChannelState(). This method may be overriden by sub-classes.

Locking: Caller must ensure that the reporter (data) lock is held.

