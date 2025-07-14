

- IOSurface
- IOSurfaceLockOptions
-  readOnly 

Type Property

# readOnly

iOS 11.0+iPadOS 11.0+Mac Catalyst 13.0+macOS 10.6+tvOS 11.0+visionOS 1.0+

``` source
static var readOnly: IOSurfaceLockOptions { get }
```

## Discussion

If you are not going to modify the data while you hold the lock, you should set this flag to avoid invalidating any existing caches of the buffer contents. This flag should be passed both to the lock and unlock functions. Non-symmentrical usage of this flag will result in undefined behavior.

## See Also

### Options

static var avoidSync: IOSurfaceLockOptions

