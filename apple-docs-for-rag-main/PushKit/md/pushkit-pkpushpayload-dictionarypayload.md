

- PushKit
- PKPushPayload
-  dictionaryPayload 

Instance Property

# dictionaryPayload

The contents of the received payload.

iOS 8.0+iPadOS 8.0+Mac Catalyst 8.0+macOS 10.15+visionOS 1.0+watchOS 6.0+

``` source
var dictionaryPayload: [AnyHashable : Any] { get }
```

## Discussion

For VoIP pushes, the sender is free to specify any fields for the contained data as long as it is provided in a text-encodable JSON format.

## See Also

### Payload Data

var type: PKPushType

The type value indicating how to interpret the payload.

