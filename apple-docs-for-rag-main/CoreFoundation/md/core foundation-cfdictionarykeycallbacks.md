

- Core Foundation
-  CFDictionaryKeyCallBacks 

Structure

# CFDictionaryKeyCallBacks

This structure contains the callbacks used to retain, release, describe, and compare the keys in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFDictionaryKeyCallBacks
```

## Topics

### Initializers

init()

init(version: CFIndex, retain: CFDictionaryRetainCallBack!, release: CFDictionaryReleaseCallBack!, copyDescription: CFDictionaryCopyDescriptionCallBack!, equal: CFDictionaryEqualCallBack!, hash: CFDictionaryHashCallBack!)

### Instance Properties

var copyDescription: CFDictionaryCopyDescriptionCallBack!

The callback used to create a descriptive string representation of each key in the dictionary. If `NULL`, the collection will create a simple description of each key. See CFDictionaryCopyDescriptionCallBack for a description of this callback.

var equal: CFDictionaryEqualCallBack!

The callback used to compare keys in the dictionary for equality. If `NULL`, the collection will use pointer equality to compare keys in the collection. See CFDictionaryEqualCallBack for a description of this callback.

var hash: CFDictionaryHashCallBack!

The callback used to compute a hash code for keys as they are used to access, add, or remove values in the dictionary. If `NULL`, the collection computes a hash code by converting the pointer value to an integer. See CFDictionaryHashCallBack for a description of this callback.

var release: CFDictionaryReleaseCallBack!

The callback used to release keys as they are removed from the dictionary. If `NULL`, keys are not released. See CFDictionaryReleaseCallBack for a description of this callback.

var retain: CFDictionaryRetainCallBack!

The callback used to retain each key as they are added to the collection. This callback returns the value to use as the key in the dictionary, which is usually the value parameter passed to this callback, but may be a different value if a different value should be used as the key. If `NULL`, keys are not retained. See CFDictionaryRetainCallBack for a descriptions of this function’s parameters.

var version: CFIndex

The version number of this structure. If not one of the defined version numbers for this opaque type, the behavior is undefined. The current version of this structure is 0.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct CFDictionaryValueCallBacks

This structure contains the callbacks used to retain, release, describe, and compare the values in a dictionary.

