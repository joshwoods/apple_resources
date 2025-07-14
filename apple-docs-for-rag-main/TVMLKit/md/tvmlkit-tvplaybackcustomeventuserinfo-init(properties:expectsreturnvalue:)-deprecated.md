

- TVMLKit
- TVPlaybackCustomEventUserInfo
-  init(properties:expectsReturnValue:) Deprecated

Initializer

# init(properties:expectsReturnValue:)

Create a new custom playback event user info dictionary.

tvOS 12.0–18.0Deprecated

``` source
init(
    properties: [TVPlaybackEventProperty : Any]?,
    expectsReturnValue: Bool
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`properties`  

A dictionary of custom playback event properties.

## Return Value

A Boolean value that indicates whether the custom playback event requires a return value.

## Discussion

When created, if the function requires a return value, it is only dispatched to first listener. Otherwise, it is broadcast to all of the listeners.

## See Also

### Creating User Info for Custom Playback Events

struct TVPlaybackEventProperty

Extend this structure to create your own custom playback event properties.

Deprecated

var expectsReturnValue: Bool

A Boolean value that indicates whether the custom event expects to contain a return value.

Deprecated

var returnValue: Any?

The return value type for the custom event.

Deprecated

