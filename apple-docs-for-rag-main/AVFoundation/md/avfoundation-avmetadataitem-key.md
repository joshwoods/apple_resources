

- AVFoundation
- AVMetadataItem
-  key 

Instance Property

# key

The key of the metadata item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
@NSCopying
var key: (any NSCopying & NSObjectProtocol)? { get }
```

## Discussion

The key property contains the true key used to identify the contents of the metadata item. This value is specific to the key space of the metadata item.

## See Also

### Accessing Keys and Key Spaces

var commonKey: AVMetadataKey?

The common key of the metadata item.

var keySpace: AVMetadataKeySpace?

The key space for the metadata item’s key.

