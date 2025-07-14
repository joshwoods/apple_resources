

- AVFoundation
- AVURLAsset
-  audiovisualMIMETypes() 

Type Method

# audiovisualMIMETypes()

Returns an array of the MIME types the asset supports.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func audiovisualMIMETypes() -> [String]
```

## Return Value

An array of MIME type strings.

## See Also

### Determining Supported Media Types

class func audiovisualTypes() -> [AVFileType]

Returns an array of the file types the asset supports.

class func isPlayableExtendedMIMEType(String) -> Bool

Returns a Boolean value that indicates whether the asset is playable with the specified codecs and container type.

