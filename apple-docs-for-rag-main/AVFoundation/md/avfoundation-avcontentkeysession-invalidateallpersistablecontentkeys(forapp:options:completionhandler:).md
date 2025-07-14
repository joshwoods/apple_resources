

- AVFoundation
- AVContentKeySession
-  invalidateAllPersistableContentKeys(forApp:options:completionHandler:) 

Instance Method

# invalidateAllPersistableContentKeys(forApp:options:completionHandler:)

Invalidates all of an app’s persistable content keys and creates a secure server playback context (SPC) to verify the outcome of an invalidation request.

iOS 12.2+iPadOS 12.2+Mac Catalyst 13.1+macOS 10.15+tvOS 17.0+visionOS 1.0+watchOS 7.0+

``` source
func invalidateAllPersistableContentKeys(
    forApp appIdentifier: Data,
    options: [AVContentKeySessionServerPlaybackContextOption : Any]? = nil,
    completionHandler handler: @escaping (Data?, (any Error)?) -> Void
)
```

``` source
func invalidateAllPersistableContentKeys(
    forApp appIdentifier: Data,
    options: [AVContentKeySessionServerPlaybackContextOption : Any]? = nil
) async throws -> Data
```

## Parameters 

`appIdentifier`  

An opaque identifier for the app.

`options`  

Additional data necessary to generate the server playback context. Pass `nil` to indicate no additional options.

See AVContentKeySessionServerPlaybackContextOption for supported options.

`handler`  

The completion handler callback.

## See Also

### Invalidating Content Keys

func invalidatePersistableContentKey(Data, options: [AVContentKeySessionServerPlaybackContextOption : Any]?, completionHandler: (Data?, (any Error)?) -> Void)

Invalidates the persistable content key and creates a secure server playback context (SPC) to verify the outcome of an invalidation request.

struct AVContentKeySessionServerPlaybackContextOption

Options for specifying additional information for generating server playback context (SPC).

