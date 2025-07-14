

- RealityKit
- AudioFileResource
-  loadAsync(named:in:inputMode:loadingStrategy:shouldLoop:) Deprecated

Type Method

# loadAsync(named:in:inputMode:loadingStrategy:shouldLoop:)

iOS 13.0–18.0DeprecatediPadOS 13.0–18.0DeprecatedMac Catalyst 13.0–18.0DeprecatedmacOS 10.15–15.0Deprecated

``` source
@MainActor @preconcurrency
static func loadAsync(
    named name: String,
    in bundle: Bundle? = nil,
    inputMode: AudioResource.InputMode = .spatial,
    loadingStrategy: AudioFileResource.LoadingStrategy = .preload,
    shouldLoop: Bool = false
) -> LoadRequest
```

## See Also

### Deprecated

static func load(named: String, in: Bundle?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) throws -> AudioFileResource

Synchronously loads an audio resource.

Deprecated

static func load(contentsOf: URL, withName: String?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) throws -> AudioFileResource

Synchronously loads an audio resource.

Deprecated

static func loadAsync(contentsOf: URL, withName: String?, inputMode: AudioResource.InputMode, loadingStrategy: AudioFileResource.LoadingStrategy, shouldLoop: Bool) -> LoadRequest&lt;AudioFileResource>Deprecated

var loadingStrategy: AudioFileResource.LoadingStrategy

The resource’s memory model.

Deprecated

var shouldLoop: Bool

Whether or not this file loops during playback. This should be set for assets that are prepared as seamless loops. A looping resource will play forever until it is explicitly told to stop.

Deprecated

