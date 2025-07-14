

- TVMLKit
-  TVPlaybackEventProperty Deprecated

Structure

# TVPlaybackEventProperty

Extend this structure to create your own custom playback event properties.

tvOS 12.0–18.0Deprecated

``` source
struct TVPlaybackEventProperty
```

Deprecated

Please use SwiftUI or UIKit

## Topics

### Initializers

init(String)

init(rawValue: String)

## Relationships

### Conforms To

- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### Creating User Info for Custom Playback Events

init(properties: [TVPlaybackEventProperty : Any]?, expectsReturnValue: Bool)

Create a new custom playback event user info dictionary.

Deprecated

var expectsReturnValue: Bool

A Boolean value that indicates whether the custom event expects to contain a return value.

Deprecated

var returnValue: Any?

The return value type for the custom event.

Deprecated

