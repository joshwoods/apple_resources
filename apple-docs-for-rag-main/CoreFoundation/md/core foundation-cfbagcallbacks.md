

- Core Foundation
-  CFBagCallBacks 

Structure

# CFBagCallBacks

This structure contains the callbacks used to retain, release, describe, and compare the values of a CFBag object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFBagCallBacks
```

## Topics

### Initializers

init()

init(version: CFIndex, retain: CFBagRetainCallBack!, release: CFBagReleaseCallBack!, copyDescription: CFBagCopyDescriptionCallBack!, equal: CFBagEqualCallBack!, hash: CFBagHashCallBack!)

### Instance Properties

var copyDescription: CFBagCopyDescriptionCallBack!

The callback used to create a descriptive string representation of each value in the collection. If `NULL`, the collection will create a simple description of each value. See CFBagCopyDescriptionCallBack for a description of this callback.

var equal: CFBagEqualCallBack!

The callback used to compare values in the collection for equality for some operations. If `NULL`, the collection will use pointer equality to compare values in the collection. See CFBagEqualCallBack for a description of this callback.

var hash: CFBagHashCallBack!

The callback used to compute a hash code for values in a collection. If `NULL`, the collection computes a hash code by converting the pointer value to an integer. See CFBagHashCallBack for a description of this callback.

var release: CFBagReleaseCallBack!

The callback used to release values as they are removed from the collection. If `NULL`, values are not released. See CFBagReleaseCallBack for a description of this callback.

var retain: CFBagRetainCallBack!

The callback used to retain each value as they are added to the collection. If `NULL`, values are not retained. See CFBagRetainCallBack for a descriptions of this function’s parameters.

var version: CFIndex

The version number of this structure. If not one of the defined version numbers for this opaque type, the behavior is undefined. The current version of this structure is 0.

## Relationships

### Conforms To

- BitwiseCopyable
- Sendable

