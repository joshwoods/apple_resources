

- AVFoundation
- AVContentKeySessionServerPlaybackContextOption
-  serverChallenge 

Type Property

# serverChallenge

Specifies a nonce to include in the secure server playback context (SPC) to prevent replay attacks.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.15+tvOS 17.0+visionOS 1.0+watchOS 7.0+

``` source
static let serverChallenge: AVContentKeySessionServerPlaybackContextOption
```

## Discussion

Specify this value as an 8-byte NSData object. If you don’t specify a value for this key, the system assumes a default server challenge of `0`.

## See Also

### Server Playback Context Options

static let protocolVersions: AVContentKeySessionServerPlaybackContextOption

Specifies the versions of the content protection protocols supported by the application.

