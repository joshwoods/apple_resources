

- AVFoundation
- AVMetadataItem
-  keySpace 

Instance Property

# keySpace

The key space for the metadata item’s key.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var keySpace: AVMetadataKeySpace? { get }
```

## Discussion

The key space that this property value specifies is typically the default key space for the metadata container that stores the metadata item.

AVFoundation uses key spaces to group related sets of keys. For example, the framework defines different key spaces for common keys, iTunes keys, ID3 keys, and QuickTime keys. Key spaces aid in filtering arrays of metadata items.

## See Also

### Accessing Keys and Key Spaces

var key: (any NSCopying &amp; NSObjectProtocol)?

The key of the metadata item.

var commonKey: AVMetadataKey?

The common key of the metadata item.

