

- Core Foundation
- CFDictionaryKeyCallBacks
-  hash 

Instance Property

# hash

The callback used to compute a hash code for keys as they are used to access, add, or remove values in the dictionary. If `NULL`, the collection computes a hash code by converting the pointer value to an integer. See CFDictionaryHashCallBack for a description of this callback.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var hash: CFDictionaryHashCallBack!
```

