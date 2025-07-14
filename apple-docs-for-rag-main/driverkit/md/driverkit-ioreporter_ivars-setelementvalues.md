

- DriverKit
- IOReporter_IVars
-  setElementValues 

Instance Method

# setElementValues

DriverKitiOSiPadOSmacOS

``` source
IOReturn setElementValues(int element_index, IOReportElementValues * values, uint64_t record_time);
```

## Parameters 

`element_index`  

- index of the \_element in internal array

`values`  

- IORepoterElementValues to replace those at \_elements\[idx\]

`record_time`  

- optional mach_absolute_time to be used for metadata

## Return Value

IOReturn code

## Discussion

Element_Index can be obtained from getFirstElementIndex(). If record_time is not provided, IOReporter::setElementValues() will fetch the current mach_absolute_time. If the current time is already known, it is more efficient to pass it along.

Locking: Caller must ensure that the reporter (data) lock is held.

