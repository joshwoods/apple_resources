

- DriverKit
- IOReporter_IVars
-  updateReportChannel 

Instance Method

# updateReportChannel

Internal method to extract channel data to a destination.

DriverKitiOSiPadOSmacOS

``` source
IOReturn updateReportChannel(int channel_index, uint32_t & elementCount, uint8_t * & buffer, size_t & capacity);
```

## Parameters 

`channel_index`  

Offset into internal elements array

`elementCount`  

Incremented by the number of IOReportElements added

`buffer`  

Buffer.

`capacity`  

Capacity.

## Return Value

Appropriate IOReturn code

## Discussion

Used to extract a single channel’s data to the updateReport() destination.

Locking: Caller must ensure that the reporter (data) lock is held.

