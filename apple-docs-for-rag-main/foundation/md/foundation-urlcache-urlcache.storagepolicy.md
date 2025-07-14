

- Foundation
- URLCache
-  URLCache.StoragePolicy 

Enumeration

# URLCache.StoragePolicy

These constants specify the caching strategy used by an CachedURLResponse object.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
enum StoragePolicy
```

## Topics

### Policies

case allowed

Storage in URLCache is allowed without restriction.

case allowedInMemoryOnly

Storage in URLCache is allowed; however storage should be restricted to memory only.

case notAllowed

Storage in URLCache is not allowed in any fashion, either in memory or on disk.

case allowed

Storage in URLCache is allowed without restriction.

case allowedInMemoryOnly

Storage in URLCache is allowed; however storage should be restricted to memory only.

case notAllowed

Storage in URLCache is not allowed in any fashion, either in memory or on disk.

### Initializers

init?(rawValue: UInt)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

