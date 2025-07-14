

- TVMLKit
- TVPlaybackEventMarshaling
-  processReturnValue(value:in:) Deprecated

Instance Method

# processReturnValue(value:in:)

Converts a JavaScript value into a value that is readable in Swift or Objective-C.

tvOS 12.0–18.0Deprecated

``` source
optional func processReturnValue(
    value: JSValue,
    in jsContext: JSContext
)
```

Deprecated

Please use SwiftUI or UIKit

## Parameters 

`value`  

A JavaScript value returned by the dispatch event.

`jsContext`  

The JavaScript context for the value.

## See Also

### Processing Playback Events

var properties: [TVPlaybackEventProperty : Any]?

An array of custom playback event properties.

**Required**

Deprecated

struct TVPlaybackEventProperty

Extend this structure to create your own custom playback event properties.

Deprecated

