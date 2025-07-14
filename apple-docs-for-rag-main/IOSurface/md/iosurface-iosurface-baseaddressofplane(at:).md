

- IOSurface
- IOSurface
-  baseAddressOfPlane(at:) 

Instance Method

# baseAddressOfPlane(at:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
func baseAddressOfPlane(at planeIndex: Int) -> UnsafeMutableRawPointer
```

## See Also

### Instance Methods

func allAttachments() -> [String : Any]?

func attachment(forKey: String) -> Any?

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

