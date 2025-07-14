

- DriverKit
- IOReporter_IVars
-  getChannelIndex 

Instance Method

# getChannelIndex

DriverKitiOSiPadOSmacOS

``` source
IOReturn getChannelIndex(uint64_t channel_id, int * channel_index);
```

## Parameters 

`channel_id`  

- ID of the channel

`channel_index`  

- pointer to the returned element_index

## Return Value

Appropriate IOReturn code

## Discussion

For efficiently and thread-safely reading channels

Locking: Caller must ensure that the reporter (data) lock is held.

