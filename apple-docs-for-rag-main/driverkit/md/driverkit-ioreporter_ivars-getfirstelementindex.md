

- DriverKit
- IOReporter_IVars
-  getFirstElementIndex 

Instance Method

# getFirstElementIndex

DriverKitiOSiPadOSmacOS

``` source
IOReturn getFirstElementIndex(uint64_t channel_id, int * element_index);
```

## Parameters 

`channel_id`  

- ID of the channel

`element_index`  

- pointer to the returned element_index

## Return Value

Appropriate IOReturn code

## Discussion

For efficiently and thread-safely reading \_elements

Locking: Caller must ensure that the reporter (data) lock is held.

