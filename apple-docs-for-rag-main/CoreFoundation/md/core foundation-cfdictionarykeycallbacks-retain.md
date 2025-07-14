

- Core Foundation
- CFDictionaryKeyCallBacks
-  retain 

Instance Property

# retain

The callback used to retain each key as they are added to the collection. This callback returns the value to use as the key in the dictionary, which is usually the value parameter passed to this callback, but may be a different value if a different value should be used as the key. If `NULL`, keys are not retained. See CFDictionaryRetainCallBack for a descriptions of this function’s parameters.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var retain: CFDictionaryRetainCallBack!
```

