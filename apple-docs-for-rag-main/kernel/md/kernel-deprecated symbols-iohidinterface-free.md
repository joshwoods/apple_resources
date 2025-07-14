

- Kernel
- Deprecated Symbols
- IOHIDInterface
-  free 

# free

Free the IOHIDInterface object.

``` source
virtual void free(); 
```

## Overview

Release all resources that were previously allocated, then call super::free() to propagate the call to our superclass.

## See Also

### Miscellaneous

init

Initialize an IOHIDInterface object.

matchPropertyTable

Called by the provider during a match

start

Start up the driver using the given provider.

