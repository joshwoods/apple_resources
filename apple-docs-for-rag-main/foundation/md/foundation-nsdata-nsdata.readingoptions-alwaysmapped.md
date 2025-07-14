

- Foundation
- NSData
- NSData.ReadingOptions
-  alwaysMapped 

Type Property

# alwaysMapped

Hint to map the file in if possible.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
static var alwaysMapped: NSData.ReadingOptions { get }
```

## Discussion

This takes precedence over mappedIfSafe if both are given.

## See Also

### Constants

static var mappedIfSafe: NSData.ReadingOptions

A hint indicating the file should be mapped into virtual memory, if possible and safe.

static var uncached: NSData.ReadingOptions

A hint indicating the file should not be stored in the file-system caches.

static var mappedIfSafe: NSData.ReadingOptions

A hint indicating the file should be mapped into virtual memory, if possible and safe.

static var uncached: NSData.ReadingOptions

A hint indicating the file should not be stored in the file-system caches.

