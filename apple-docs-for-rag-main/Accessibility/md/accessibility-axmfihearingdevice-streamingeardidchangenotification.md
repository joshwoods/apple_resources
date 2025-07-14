

- Accessibility
- AXMFiHearingDevice
-  streamingEarDidChangeNotification 

Type Property

# streamingEarDidChangeNotification

A notification that the system posts when there’s a change to which ears enable streaming.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
static let streamingEarDidChangeNotification: NSNotification.Name
```

## Discussion

The system posts this notification when the value of streamingEar() changes.

## See Also

### Streaming status

struct Ear

Constants that represent a hearing device ear.

static func streamingEar() -> AXMFiHearingDevice.Ear

Returns which ears enable streaming.

