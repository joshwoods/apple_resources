

- DriverKit
- OSArray
-  ensureCapacity 

Instance Method

# ensureCapacity

Allocates capacity for members in array.

DriverKitiOSiPadOSmacOS

``` source
uint32_t ensureCapacity(uint32_t newCapacity);
```

## Parameters 

`newCapacity`  

Count of allocated capacity for members in array.

## Return Value

New count of capacity for members in array, may return prior capacity on failure.

## See Also

### Inspecting an Array

getCount

Returns count of members in array.

getCapacity

Returns count of currently allocated capacity for members in array.

OSArrayGetCount

