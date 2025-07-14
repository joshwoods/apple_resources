

- Accessibility
- AXMFiHearingDevice
-  streamingEar() 

Type Method

# streamingEar()

Returns which ears enable streaming.

iOS 15.0+iPadOS 15.0+Mac Catalyst 15.0+visionOS 1.0+watchOS 8.0+

``` source
static func streamingEar() -> AXMFiHearingDevice.Ear
```

## Return Value

An AXMFiHearingDevice.Ear constant that represents which ears enable streaming.

## See Also

### Streaming status

struct Ear

Constants that represent a hearing device ear.

static let streamingEarDidChangeNotification: NSNotification.Name

A notification that the system posts when there’s a change to which ears enable streaming.

