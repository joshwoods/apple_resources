

- Core Foundation
-  CFArrayCallBacks 

Structure

# CFArrayCallBacks

Structure containing the callbacks of a CFArray.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFArrayCallBacks
```

## Topics

### Initializers

init()

init(version: CFIndex, retain: CFArrayRetainCallBack!, release: CFArrayReleaseCallBack!, copyDescription: CFArrayCopyDescriptionCallBack!, equal: CFArrayEqualCallBack!)

### Instance Properties

var copyDescription: CFArrayCopyDescriptionCallBack!

The callback used to create a descriptive string representation of each value in the collection. If `NULL`, the collection will create a simple description of each value. See CFArrayCopyDescriptionCallBack for a description of this callback.

var equal: CFArrayEqualCallBack!

The callback used to compare values in the array for equality for some operations. If `NULL`, the collection will use pointer equality to compare values in the collection. See CFArrayEqualCallBack for a description of this callback.

var release: CFArrayReleaseCallBack!

The callback used to release values as they are removed from the collection. If `NULL`, values are not released. See CFArrayReleaseCallBack for a description of this callback.

var retain: CFArrayRetainCallBack!

The callback used to retain each value as they are added to the collection. If `NULL`, values are not retained. See CFArrayRetainCallBack for a description of this callback.

var version: CFIndex

The version number of this structure. If not one of the defined version numbers for this opaque type, the behavior is undefined. The current version of this structure is 0.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

