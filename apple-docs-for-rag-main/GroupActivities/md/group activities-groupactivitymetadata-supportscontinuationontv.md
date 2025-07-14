

- Group Activities
- GroupActivityMetadata
-  supportsContinuationOnTV 

Instance Property

# supportsContinuationOnTV

A Boolean value that indicates whether your app supports activity continuation on an Apple TV.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+macOS 12.0+tvOS 15.0+visionOS 1.0+

``` source
var supportsContinuationOnTV: Bool
```

## Discussion

The default value of this property is `false`. Set it to `true` to allow participants to continue the activity on Apple TV.

## See Also

### Specifying media-related behavior

var preferredBroadcastOptions: BroadcastOptions

Preferences for how to present audio and video on the main communication channel.

struct BroadcastOptions

Options for how to broadcast media on the shared communications channel.

