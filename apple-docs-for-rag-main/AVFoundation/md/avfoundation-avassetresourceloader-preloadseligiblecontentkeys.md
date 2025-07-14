

- AVFoundation
- AVAssetResourceLoader
-  preloadsEligibleContentKeys 

Instance Property

# preloadsEligibleContentKeys

A Boolean value that indicates whether content keys will be loaded as quickly as possible.

iOS 9.0+iPadOS 9.0+Mac Catalyst 13.1+macOS 10.11+tvOS 9.0+visionOS 1.0+

``` source
var preloadsEligibleContentKeys: Bool { get set }
```

## Discussion

Set this property to `true` to load eligible keys. This may result in network activity. All work done as a result of setting this property to `true` is performed asynchronously.

