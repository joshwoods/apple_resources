

- Kernel
- IOKit Fundamentals
- Memory
- IODeviceMemory
-  arrayFromList 

# arrayFromList

Constructs an OSArray of IODeviceMemory instances, each describing one physical range, and a tag value.

``` source
static OSArray * arrayFromList( 
 InitElement list[], 
 IOItemCount count ); 
```

## Parameters 

`list`  

An array of IODeviceMemory::InitElement structures.

`count`  

The number of elements in the list.

## Return Value

Returns a created OSArray of IODeviceMemory objects, to be released by the caller, or zero on failure.

## Overview

This method creates IODeviceMemory instances for each physical range passed in an IODeviceMemory::InitElement array. Each element consists of a physical address, length and tag value for the IODeviceMemory. The instances are returned as a created OSArray.

## See Also

### Miscellaneous

withRange

Constructs an IODeviceMemory instance, describing one physical range.

withSubRange

Constructs an IODeviceMemory instance, describing a subset of an existing IODeviceMemory range.

