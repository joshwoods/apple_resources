

- AVFoundation
- AVURLAsset
-  isPlayableExtendedMIMEType(\_:) 

Type Method

# isPlayableExtendedMIMEType(\_:)

Returns a Boolean value that indicates whether the asset is playable with the specified codecs and container type.

iOS 5.0+iPadOS 5.0+Mac Catalyst 13.1+macOS 10.7+tvOS 9.0+visionOS 1.0+watchOS 1.0+

``` source
class func isPlayableExtendedMIMEType(_ extendedMIMEType: String) -> Bool
```

## Parameters 

`extendedMIMEType`  

An extended MIME type string such as `video/3gpp2; codecs=“mp4v.20.9, mp4a.E1”` or `audio/aac; codecs=“mp4a.E1”`.

## Return Value

true if the asset is playable with the specified codec and container type; otherwise, false.

## See Also

### Determining Supported Media Types

class func audiovisualTypes() -> [AVFileType]

Returns an array of the file types the asset supports.

class func audiovisualMIMETypes() -> [String]

Returns an array of the MIME types the asset supports.

