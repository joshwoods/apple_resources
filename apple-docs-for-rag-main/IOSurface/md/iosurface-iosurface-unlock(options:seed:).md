

- IOSurface
- IOSurface
-  unlock(options:seed:) 

Instance Method

# unlock(options:seed:)

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.1+macOS 10.12+tvOS 11.0+visionOS 1.0+

``` source
func unlock(
    options: IOSurfaceLockOptions = [],
    seed: UnsafeMutablePointer?
) -> kern_return_t
```

## See Also

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

