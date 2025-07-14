

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  start 

# start

Start up the driver using the given provider.

``` source
virtual bool start(
 IOService *provider ); 
```

## Parameters 

`provider`  

The provider that the driver was matched to, and selected to run with.

## Return Value

True on success, or false otherwise.

## Overview

IOHIDInterface will allocate resources. Before returning true to indicate success, registerService() is called to trigger client matching.

## See Also

### Miscellaneous

free

Free the IOHIDInterface object.

init

Initialize an IOHIDInterface object.

matchPropertyTable

Called by the provider during a match

