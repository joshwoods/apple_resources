

- AVFoundation
-  AVAssetReferenceRestrictions 

Structure

# AVAssetReferenceRestrictions

Restrictions to use when resolving references to external media data.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVAssetReferenceRestrictions
```

## Topics

### Reference Restrictions

static var forbidAll: AVAssetReferenceRestrictions

The asset can only reference media stored within its container file.

static var forbidRemoteReferenceToLocal: AVAssetReferenceRestrictions

A remote asset shouldn’t follow references to local media.

static var forbidLocalReferenceToRemote: AVAssetReferenceRestrictions

A local asset shouldn’t follow references to remote media.

static var forbidCrossSiteReference: AVAssetReferenceRestrictions

A remote asset shouldn’t follow references to remote media data stored at a different host.

static var forbidLocalReferenceToLocal: AVAssetReferenceRestrictions

A local asset shouldn’t follow references to local media data stored outside its container file.

static var defaultPolicy: AVAssetReferenceRestrictions

The asset should use the default reference restrictions policy.

### Initializers

init(rawValue: UInt)

Creates reference restrictions with an integer value.

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- ExpressibleByArrayLiteral
- OptionSet
- RawRepresentable
- Sendable
- SetAlgebra

## See Also

### Retrieving Reference Restrictions

var referenceRestrictions: AVAssetReferenceRestrictions

The restrictions that an asset places on how it resolves references to external media.

