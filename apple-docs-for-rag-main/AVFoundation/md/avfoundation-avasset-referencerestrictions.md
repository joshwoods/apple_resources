

- AVFoundation
- AVAsset
-  referenceRestrictions 

Instance Property

# referenceRestrictions

The restrictions that an asset places on how it resolves references to external media.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+

``` source
var referenceRestrictions: AVAssetReferenceRestrictions { get }
```

## Discussion

For AVURLAsset, this property reflects the value passed in for AVURLAssetReferenceRestrictionsKey, if any.

The default value for this property is defaultPolicy. See AVURLAssetReferenceRestrictionsKey for more information about reference restrictions.

## See Also

### Retrieving Reference Restrictions

struct AVAssetReferenceRestrictions

Restrictions to use when resolving references to external media data.

