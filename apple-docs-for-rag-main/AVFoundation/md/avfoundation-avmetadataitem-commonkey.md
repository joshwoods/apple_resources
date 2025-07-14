

- AVFoundation
- AVMetadataItem
-  commonKey 

Instance Property

# commonKey

The common key of the metadata item.

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
var commonKey: AVMetadataKey? { get }
```

## Discussion

This value contains the key that most closely corresponds to the key property, but that belongs to the common key space. You can use this key to locate metadata items irrespective of the underlying media format.

If the value of the keySpace property is common, this property value contains the same key as the key property.

## See Also

### Accessing Keys and Key Spaces

var key: (any NSCopying &amp; NSObjectProtocol)?

The key of the metadata item.

var keySpace: AVMetadataKeySpace?

The key space for the metadata item’s key.

