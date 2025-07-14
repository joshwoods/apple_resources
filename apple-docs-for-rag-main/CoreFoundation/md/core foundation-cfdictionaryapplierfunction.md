

- Core Foundation
-  CFDictionaryApplierFunction 

Type Alias

# CFDictionaryApplierFunction

Prototype of a callback function that may be applied to every key-value pair in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
typealias CFDictionaryApplierFunction = (UnsafeRawPointer?, UnsafeRawPointer?, UnsafeMutableRawPointer?) -> Void
```

## Parameters 

`key`  

The key associated with the current key-value pair.

`value`  

The value associated with the current key-value pair.

`context`  

The program-defined context parameter given to the apply function.

## Discussion

This callback is passed to the CFDictionaryApplyFunction(_:_:_:) function which iterates over the key-value pairs in a dictionary and applies the behavior defined in the applier function to each key-value pair in a dictionary.

## See Also

### Callbacks

typealias CFDictionaryCopyDescriptionCallBack

Prototype of a callback function used to get a description of a value or key in a dictionary.

typealias CFDictionaryEqualCallBack

Prototype of a callback function used to determine if two values or keys in a dictionary are equal.

typealias CFDictionaryHashCallBack

Prototype of a callback function invoked to compute a hash code for a key. Hash codes are used when key-value pairs are accessed, added, or removed from a collection.

typealias CFDictionaryReleaseCallBack

Prototype of a callback function used to release a key-value pair before it’s removed from a dictionary.

typealias CFDictionaryRetainCallBack

Prototype of a callback function used to retain a value or key being added to a dictionary.

