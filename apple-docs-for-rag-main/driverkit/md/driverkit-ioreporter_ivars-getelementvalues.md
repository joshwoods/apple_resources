

- DriverKit
- IOReporter_IVars
-  getElementValues 

Instance Method

# getElementValues

DriverKitiOSiPadOSmacOS

``` source
const IOReportElementValues * getElementValues(int element_index);
```

## Parameters 

`element_index`  

- index of the \_element in internal array

## Return Value

A pointer to the element values requested or NULL on failure

## Discussion

Locking: Caller must ensure that the reporter (data) lock is held. The returned pointer is only valid until unlockReporter() is called.

