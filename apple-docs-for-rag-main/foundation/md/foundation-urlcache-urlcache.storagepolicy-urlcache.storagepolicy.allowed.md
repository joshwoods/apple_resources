

- Foundation
- URLCache
- URLCache.StoragePolicy
-  URLCache.StoragePolicy.allowed 

Case

# URLCache.StoragePolicy.allowed

Storage in URLCache is allowed without restriction.

iOS 2.0+iPadOS 2.0+Mac Catalyst 13.0+macOS 10.0+tvOS 9.0+visionOS 1.0+watchOS 2.0+

``` source
case allowed
```

## Discussion

Important

iOS prior to version 5 ignores this cache policy, and instead treats it as URLCache.StoragePolicy.allowedInMemoryOnly.

## See Also

### Policies

case allowedInMemoryOnly

Storage in URLCache is allowed; however storage should be restricted to memory only.

case notAllowed

Storage in URLCache is not allowed in any fashion, either in memory or on disk.

case allowedInMemoryOnly

Storage in URLCache is allowed; however storage should be restricted to memory only.

case notAllowed

Storage in URLCache is not allowed in any fashion, either in memory or on disk.

