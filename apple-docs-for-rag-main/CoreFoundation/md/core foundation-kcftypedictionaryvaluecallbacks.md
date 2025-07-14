

- Core Foundation
-  kCFTypeDictionaryValueCallBacks 

Global Variable

# kCFTypeDictionaryValueCallBacks

Predefined CFDictionaryValueCallBacks structure containing a set of callbacks appropriate for use when the values in a CFDictionary are all CFType-derived objects.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFTypeDictionaryValueCallBacks: CFDictionaryValueCallBacks
```

## Discussion

The retain callback is `CFRetain`, the release callback is `CFRelease`, the copy callback is `CFCopyDescription`, and the equal callback is `CFEqual`. Therefore, if you use a pointer to this constant when creating the dictionary, values are automatically retained when added to the collection, and released when removed from the collection.

## See Also

### Constants

let kCFCopyStringDictionaryKeyCallBacks: CFDictionaryKeyCallBacks

Predefined CFDictionaryKeyCallBacks structure containing a set of callbacks appropriate for use when the keys of a CFDictionary are all CFString objects, which may be mutable and need to be copied in order to serve as constant keys for the values in the dictionary.

let kCFTypeDictionaryKeyCallBacks: CFDictionaryKeyCallBacks

Predefined CFDictionaryKeyCallBacks structure containing a set of callbacks appropriate for use when the keys of a CFDictionary are all CFType-derived objects.

