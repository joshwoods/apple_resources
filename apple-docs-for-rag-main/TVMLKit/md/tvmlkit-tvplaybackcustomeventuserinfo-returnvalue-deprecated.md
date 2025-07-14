

- TVMLKit
- TVPlaybackCustomEventUserInfo
-  returnValue Deprecated

Instance Property

# returnValue

The return value type for the custom event.

tvOS 12.0–18.0Deprecated

``` source
var returnValue: Any? { get }
```

Deprecated

Please use SwiftUI or UIKit

## See Also

### Creating User Info for Custom Playback Events

init(properties: [TVPlaybackEventProperty : Any]?, expectsReturnValue: Bool)

Create a new custom playback event user info dictionary.

Deprecated

struct TVPlaybackEventProperty

Extend this structure to create your own custom playback event properties.

Deprecated

var expectsReturnValue: Bool

A Boolean value that indicates whether the custom event expects to contain a return value.

Deprecated

