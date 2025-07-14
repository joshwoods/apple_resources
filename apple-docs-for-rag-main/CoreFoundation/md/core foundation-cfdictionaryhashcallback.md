

- Core Foundation
-  CFDictionaryHashCallBack 

Type Alias

# CFDictionaryHashCallBack

Prototype of a callback function invoked to compute a hash code for a key. Hash codes are used when key-value pairs are accessed, added, or removed from a collection.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFDictionaryHashCallBack = (UnsafeRawPointer?) -> CFHashCode
```

## Parameters 

`value`  

The value used to compute the hash code.

## Return Value

An integer that can be used as a table address in a hash table structure.

## Discussion

This callback is passed to CFDictionaryCreate(_:_:_:_:_:_:) in a CFDictionaryKeyCallBacks structure.

## See Also

### Callbacks

typealias CFDictionaryApplierFunction

Prototype of a callback function that may be applied to every key-value pair in a dictionary.

typealias CFDictionaryCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value or key in a dictionary.

typealias CFDictionaryEqualCallBack

Prototype of a callback function used to determine if two values or keys in a dictionary are equal.

typealias CFDictionaryReleaseCallBack

Prototype of a callback function used to release a key-value pair before it’s removed from a dictionary.

typealias CFDictionaryRetainCallBack

Prototype of a callback function used to retain a value or key being added to a dictionary.

