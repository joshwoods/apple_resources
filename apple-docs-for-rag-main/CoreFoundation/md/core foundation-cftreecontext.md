

- Core Foundation
-  CFTreeContext 

Structure

# CFTreeContext

Structure containing program-defined data and callbacks for a CFTree object.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFTreeContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: CFTreeRetainCallBack!, release: CFTreeReleaseCallBack!, copyDescription: CFTreeCopyDescriptionCallBack!)

### Instance Properties

var copyDescription: CFTreeCopyDescriptionCallBack!

The callback used to provide a description of the `info` field.

var info: UnsafeMutableRawPointer!

A C pointer to a program-defined block of data, referred to as the information pointer.

var release: CFTreeReleaseCallBack!

The callback used to release a previously retained `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. This value may be `NULL`.

var retain: CFTreeRetainCallBack!

The callback used to retain the `info` field. If this parameter is not a pointer to a function of the correct prototype, the behavior is undefined. This value may be `NULL`.

var version: CFIndex

The version number of the structure type being passed in as a parameter to a CFTree creation function. This structure is version `0`.

## Relationships

### Conforms To

- BitwiseCopyable

