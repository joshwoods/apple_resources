

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  init 

# init

Initialize an IOHIDInterface object.

``` source
virtual bool init(
 OSDictionary *dictionary = 0 ); 
```

## Parameters 

`A`  

dictionary A property table associated with this IOHIDInterface instance.

## Return Value

True on sucess, or false otherwise.

## Overview

Prime the IOHIDInterface object and prepare it to support a probe() or a start() call. This implementation will simply call super::init().

## See Also

### Miscellaneous

free

Free the IOHIDInterface object.

matchPropertyTable

Called by the provider during a match

start

Start up the driver using the given provider.

