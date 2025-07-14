

- AVFoundation
-  AVContentKeySystem 

Structure

# AVContentKeySystem

A key-delivery method for a content key session.

iOS 10.3+iPadOS 10.3+Mac Catalyst 13.1+macOS 10.12.4+tvOS 10.2+visionOS 1.0+watchOS 7.0+

``` source
struct AVContentKeySystem
```

## Topics

### Key-Delivery Methods

static let fairPlayStreaming: AVContentKeySystem

A method of key delivery that uses FairPlay Streaming.

static let clearKey: AVContentKeySystem

A method of key delivery that uses a clear key system.

static let authorizationToken: AVContentKeySystem

A method of key delivery that uses a token to authorize playback.

### Initializers

init(rawValue: String)

Creates a content key system with a string value.

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Inspecting the Session

var keySystem: AVContentKeySystem

The type of key system used to retrieve keys.

var storageURL: URL?

A URL that points to a writable storage directory.

