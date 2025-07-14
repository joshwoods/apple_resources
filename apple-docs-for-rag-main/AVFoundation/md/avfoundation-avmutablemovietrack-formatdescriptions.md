

- AVFoundation
- AVMutableMovieTrack
-  formatDescriptions 

Instance Property

# formatDescriptions

The format descriptions of the media samples that a track references.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.11+visionOS 1.0+watchOS 6.0+

``` source
var formatDescriptions: [Any] { get }
```

## Discussion

The array contains CMFormatDescription objects that indicate the format of media samples the track references.

Asset tracks typically present uniform media (for example, media that uses the same encoding settings) and contain a single format description. However, in some cases, an asset track may contain multiple format descriptions. For example, an H.264-encoded video track may have some segments that use the Main profile and others that use the High profile. Also, an individual AVCompositionTrack, which subclasses AVAssetTrack, may contain audio or video segments using different codecs.

You can use CMFormatDescription to access low-level details about the media the track references. For example, you can retrieve the details of track’s media type and subtype as the code below shows:

```
extension AVAssetTrack {
    var mediaFormat: String {
        get async throws {
            var format = ""
            let descriptions = try await load(.formatDescriptions)
            for (index, formatDesc) in descriptions.enumerated() {
                // Get a string representation of the media type.
                let type =
                    CMFormatDescriptionGetMediaType(formatDesc).toString()
                // Get a string representation of the media subtype.
                let subType =
                    CMFormatDescriptionGetMediaSubType(formatDesc).toString()
                // Format the string as type/subType, such as vide/avc1 or soun/aac.
                format += "\(type)/\(subType)"
                // Comma-separate if there's more than one format description.
                if index  String {
        let bytes: [CChar] = [
            CChar((self >> 24) & 0xff),
            CChar((self >> 16) & 0xff),
            CChar((self >> 8) & 0xff),
            CChar(self & 0xff),
            0
        ]
        let result = String(cString: bytes)
        let characterSet = CharacterSet.whitespaces
        return result.trimmingCharacters(in: characterSet)
    }
}
```

## See Also

### Changing Format Descriptions

func replaceFormatDescription(CMFormatDescription, with: CMFormatDescription)

Replaces the track’s format description with a new format description.

