

- Core Foundation
-  CFDictionaryRetainCallBack 

Type Alias

# CFDictionaryRetainCallBack

Prototype of a callback function used to retain a value or key being added to a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFDictionaryRetainCallBack = (CFAllocator?, UnsafeRawPointer?) -> UnsafeRawPointer?
```

## Parameters 

`allocator`  

The dictionary’s allocator.

`value`  

The value being added to the dictionary.

## Return Value

The value or key to store in the dictionary, which is usually the `value` parameter passed to this callback, but may be a different value if a different value should be stored in the collection.

## Discussion

This callback is passed to CFDictionaryCreate(_:_:_:_:_:_:) in a CFDictionaryKeyCallBacks and CFDictionaryValueCallBacks structure.

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

typealias CFDictionaryReleaseCallBack

Prototype of a callback function used to release a key-value pair before it’s removed from a dictionary.

