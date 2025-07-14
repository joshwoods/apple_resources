

- DriverKit
- OSDictionary
-  ensureCapacity 

Instance Method

# ensureCapacity

Allocates capacity for members in dictionary.

DriverKitiOSiPadOSmacOS

``` source
uint32_t ensureCapacity(uint32_t newCapacity);
```

## Parameters 

`newCapacity`  

Count of allocated capacity for members in dictionary.

## Return Value

New count of capacity for members in dictionary, may return prior capacity on failure.

## See Also

### Inspecting a Dictionary

getCapacity

Returns count of currently allocated capacity for members in dictionary.

getCount

Returns count of members in dictionary.

OSDictionaryGetCount

