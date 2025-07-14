

- Core Foundation
-  CFDictionaryReleaseCallBack 

Type Alias

# CFDictionaryReleaseCallBack

Prototype of a callback function used to release a key-value pair before it’s removed from a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFDictionaryReleaseCallBack = (CFAllocator?, UnsafeRawPointer?) -> Void
```

## Parameters 

`allocator`  

The dictionary’s allocator.

`value`  

The value being removed from the dictionary.

## See Also

### Callbacks

typealias CFDictionaryApplierFunction

Prototype of a callback function that may be applied to every key-value pair in a dictionary.

typealias CFDictionaryCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value or key in a dictionary.

typealias CFDictionaryEqualCallBack

Prototype of a callback function used to determine if two values or keys in a dictionary are equal.

typealias CFDictionaryHashCallBack

Prototype of a callback function invoked to compute a hash code for a key. Hash codes are used when key-value pairs are accessed, added, or removed from a collection.

typealias CFDictionaryRetainCallBack

Prototype of a callback function used to retain a value or key being added to a dictionary.

