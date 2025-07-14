

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  matchPropertyTable 

# matchPropertyTable

Called by the provider during a match

``` source
virtual bool matchPropertyTable( 
 OSDictionary *table, 
 SInt32 *score); 
```

## Parameters 

`table`  

The property table that this device will match against

## Overview

Compare the properties in the supplied table to this object's properties.

## See Also

### Miscellaneous

free

Free the IOHIDInterface object.

init

Initialize an IOHIDInterface object.

start

Start up the driver using the given provider.

