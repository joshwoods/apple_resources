

- AVFoundation
- AVPartialAsyncProperty
-  formatDescriptions 

Type Property

# formatDescriptions

The format descriptions of the media samples that a track references.

iOS 15.0+iPadOS 15.0+Mac CatalystmacOS 12.0+tvOS 15.0+visionOS 1.0+watchOS 8.0+

``` source
static var formatDescriptions: AVAsyncProperty { get }
```

Available when `Root` inherits `AVAssetTrack`.

## Discussion

Use the load(_:) method to retrieve the property value.

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
                let type = CMFormatDescriptionGetMediaType(formatDesc).toString()
                // Get a string representation of the media subtype.
                let subType = CMFormatDescriptionGetMediaSubType(formatDesc).toString()
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

### Loading Track Information

static var isPlayable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is playable in the current environment.

static var isDecodable: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is decodable in the current environment.

static var isEnabled: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track is in an enabled state.

static var isSelfContained: AVAsyncProperty&lt;Root, Bool>

A Boolean value that indicates whether the track references sample data only within its container file.

static var totalSampleDataLength: AVAsyncProperty&lt;Root, Int64>

The total number of bytes of sample data the track requires.

static var mediaCharacteristics: AVAsyncProperty&lt;Root, [AVMediaCharacteristic]>

The media characteristics for the track.

