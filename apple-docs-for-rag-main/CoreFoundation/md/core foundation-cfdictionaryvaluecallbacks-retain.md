

- Core Foundation
- CFDictionaryValueCallBacks
-  retain 

Instance Property

# retain

The callback used to retain each value as they are added to the collection. This callback returns the value to use as the value in the dictionary, which is usually the value parameter passed to this callback, but may be a different value if a different value should be used as the value. If `NULL`, values are not retained. See CFDictionaryRetainCallBack for a descriptions of this function’s parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var retain: CFDictionaryRetainCallBack!
```

