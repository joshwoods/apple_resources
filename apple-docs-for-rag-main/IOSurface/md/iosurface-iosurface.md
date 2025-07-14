

- IOSurface
-  IOSurface 

Class

# IOSurface

Data type representing an IOSurface opaque object.

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
class IOSurface
```

## Topics

### Initializers

init?(properties: [IOSurfacePropertyKey : Any])

### Instance Properties

var allocationSize: Int

var allowsPixelSizeCasting: Bool

var baseAddress: UnsafeMutableRawPointer

var bytesPerElement: Int

var bytesPerRow: Int

var elementHeight: Int

var elementWidth: Int

var height: Int

var isInUse: Bool

var localUseCount: Int32

var pixelFormat: OSType

var planeCount: Int

var seed: UInt32

var width: Int

var surfaceID: UInt32

### Instance Methods

func allAttachments() -> [String : Any]?

func attachment(forKey: String) -> Any?

func baseAddressOfPlane(at: Int) -> UnsafeMutableRawPointer

func bytesPerElementOfPlane(at: Int) -> Int

func bytesPerRowOfPlane(at: Int) -> Int

func decrementUseCount()

func elementHeightOfPlane(at: Int) -> Int

func elementWidthOfPlane(at: Int) -> Int

func heightOfPlane(at: Int) -> Int

func incrementUseCount()

func lock(options: IOSurfaceLockOptions, seed: UnsafeMutablePointer&lt;UInt32>?) -> kern_return_t

func removeAllAttachments()

func removeAttachment(forKey: String)

func setAllAttachments([String : Any])

func setAttachment(Any, forKey: String)

func setPurgeable(IOSurfacePurgeabilityState, oldState: UnsafeMutablePointer&lt;IOSurfacePurgeabilityState>?) -> kern_return_t

func unlock(options: IOSurfaceLockOptions, seed: UnsafeMutablePointer&lt;UInt32>?) -> kern_return_t

func widthOfPlane(at: Int) -> Int

## Relationships

### Inherits From

- NSObject

### Conforms To

- CVarArg
- CustomDebugStringConvertible
- CustomStringConvertible
- Equatable
- Hashable
- NSCoding
- NSObjectProtocol
- NSSecureCoding

## See Also

### Classes

class IOSurfaceRef

Data type representing an IOSurface opaque object.

