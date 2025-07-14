

- AVFoundation
-  AVContentKeySessionServerPlaybackContextOption 

Structure

# AVContentKeySessionServerPlaybackContextOption

Options for specifying additional information for generating server playback context (SPC).

iOSiPadOSMac CatalystmacOStvOSvisionOSwatchOS

``` source
struct AVContentKeySessionServerPlaybackContextOption
```

## Topics

### Server Playback Context Options

static let protocolVersions: AVContentKeySessionServerPlaybackContextOption

Specifies the versions of the content protection protocols supported by the application.

static let serverChallenge: AVContentKeySessionServerPlaybackContextOption

Specifies a nonce to include in the secure server playback context (SPC) to prevent replay attacks.

### Initializing an Options Structure

init(rawValue: String)

Creates a playback context options structure with the specified raw value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Invalidating Content Keys

func invalidatePersistableContentKey(Data, options: [AVContentKeySessionServerPlaybackContextOption : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Invalidates the persistable content key and creates a secure server playback context (SPC) to verify the outcome of an invalidation request.

func invalidateAllPersistableContentKeys(forApp: Data, options: [AVContentKeySessionServerPlaybackContextOption : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Invalidates all of an app’s persistable content keys and creates a secure server playback context (SPC) to verify the outcome of an invalidation request.

