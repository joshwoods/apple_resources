

- Core Foundation
-  kCFCopyStringDictionaryKeyCallBacks 

Global Variable

# kCFCopyStringDictionaryKeyCallBacks

Predefined CFDictionaryKeyCallBacks structure containing a set of callbacks appropriate for use when the keys of a CFDictionary are all CFString objects, which may be mutable and need to be copied in order to serve as constant keys for the values in the dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
let kCFCopyStringDictionaryKeyCallBacks: CFDictionaryKeyCallBacks
```

## Discussion

You typically use a pointer to this constant when creating a new dictionary.

Important

For performance reasons, the default `kCFCopyStringDictionaryKeyCallBacks` behavior uses CFEqual(_:_:) which does not normalize the strings. This means that, for example, it does not consider CFStrings to be equal when they are the same but one is in pre-composed form (say, originating from a UTF-16 text file) and the other in decomposed form (say, originating from a file name). In cases where you use strings from different sources, you may want to pre-normalize the keys or else use a different set of functions to perform the comparison.

## See Also

### Constants

let kCFTypeDictionaryKeyCallBacks: CFDictionaryKeyCallBacks

Predefined CFDictionaryKeyCallBacks structure containing a set of callbacks appropriate for use when the keys of a CFDictionary are all CFType-derived objects.

let kCFTypeDictionaryValueCallBacks: CFDictionaryValueCallBacks

Predefined CFDictionaryValueCallBacks structure containing a set of callbacks appropriate for use when the values in a CFDictionary are all CFType-derived objects.

