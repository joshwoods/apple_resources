

- Core Foundation
-  CFDictionaryValueCallBacks 

Structure

# CFDictionaryValueCallBacks

This structure contains the callbacks used to retain, release, describe, and compare the values in a dictionary.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFDictionaryValueCallBacks
```

## Topics

### Initializers

init()

init(version: CFIndex, retain: CFDictionaryRetainCallBack!, release: CFDictionaryReleaseCallBack!, copyDescription: CFDictionaryCopyDescriptionCallBack!, equal: CFDictionaryEqualCallBack!)

### Instance Properties

var copyDescription: CFDictionaryCopyDescriptionCallBack!

The callback used to create a descriptive string representation of each value in the dictionary. If `NULL`, the collection will create a simple description of each value. See CFDictionaryCopyDescriptionCallBack for a description of this callback.

var equal: CFDictionaryEqualCallBack!

The callback used to compare values in the dictionary for equality. If `NULL`, the collection will use pointer equality to compare values in the collection. See CFDictionaryEqualCallBack for a description of this callback.

var release: CFDictionaryReleaseCallBack!

The callback used to release values as they are removed from the dictionary. If `NULL`, values are not released. See CFDictionaryReleaseCallBack for a description of this callback.

var retain: CFDictionaryRetainCallBack!

The callback used to retain each value as they are added to the collection. This callback returns the value to use as the value in the dictionary, which is usually the value parameter passed to this callback, but may be a different value if a different value should be used as the value. If `NULL`, values are not retained. See CFDictionaryRetainCallBack for a descriptions of this function’s parameters.

var version: CFIndex

The version number of this structure. If not one of the defined version numbers for this opaque type, the behavior is undefined. The current version of this structure is 0.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

## See Also

### Data Types

struct CFDictionaryKeyCallBacks

This structure contains the callbacks used to retain, release, describe, and compare the keys in a dictionary.

