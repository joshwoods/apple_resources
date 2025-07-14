

- AVFoundation
- AVAssetReferenceRestrictions
-  forbidCrossSiteReference 

Type Property

# forbidCrossSiteReference

A remote asset shouldn’t follow references to remote media data stored at a different host.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
static var forbidCrossSiteReference: AVAssetReferenceRestrictions { get }
```

## See Also

### Reference Restrictions

static var forbidAll: AVAssetReferenceRestrictions

The asset can only reference media stored within its container file.

static var forbidRemoteReferenceToLocal: AVAssetReferenceRestrictions

A remote asset shouldn’t follow references to local media.

static var forbidLocalReferenceToRemote: AVAssetReferenceRestrictions

A local asset shouldn’t follow references to remote media.

static var forbidLocalReferenceToLocal: AVAssetReferenceRestrictions

A local asset shouldn’t follow references to local media data stored outside its container file.

static var defaultPolicy: AVAssetReferenceRestrictions

The asset should use the default reference restrictions policy.

