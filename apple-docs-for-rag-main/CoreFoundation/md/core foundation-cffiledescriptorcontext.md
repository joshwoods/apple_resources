

- Core Foundation
-  CFFileDescriptorContext 

Structure

# CFFileDescriptorContext

Defines a structure for the context of a CFFileDescriptor.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct CFFileDescriptorContext
```

## Topics

### Initializers

init()

init(version: CFIndex, info: UnsafeMutableRawPointer!, retain: ((UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!, release: ((UnsafeMutableRawPointer?) -> Void)!, copyDescription: ((UnsafeMutableRawPointer?) -> Unmanaged&lt;CFString>?)!)

### Instance Properties

var copyDescription: ((UnsafeMutableRawPointer?) -> Unmanaged&lt;CFString>?)!

The callback used to create a descriptive string representation of the CFFileDescriptor.

var info: UnsafeMutableRawPointer!

var release: ((UnsafeMutableRawPointer?) -> Void)!

The release callback used by the CFFileDescriptor.

var retain: ((UnsafeMutableRawPointer?) -> UnsafeMutableRawPointer?)!

The retain callback used by the CFFileDescriptor.

var version: CFIndex

The version number of this structure. If not one of the defined version numbers for this opaque type, the behavior is undefined. The current version of this structure is 0.

## Relationships

### Conforms To

- BitwiseCopyable

## See Also

### Data Types

typealias CFFileDescriptorNativeDescriptor

Defines a type for the native file descriptor.

typealias CFFileDescriptorCallBack

Defines a structure for a callback for a CFFileDescriptor.

