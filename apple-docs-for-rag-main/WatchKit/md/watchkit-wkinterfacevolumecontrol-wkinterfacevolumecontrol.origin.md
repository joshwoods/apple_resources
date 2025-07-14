

- WatchKit
- WKInterfaceVolumeControl
-  WKInterfaceVolumeControl.Origin 

Enumeration

# WKInterfaceVolumeControl.Origin

The source of the audio managed by the volume control.

watchOS 6.0+

``` source
enum Origin
```

## Topics

### Audio Sources

case companion

Audio playing on iPhone.

case local

Audio playing on Apple Watch.

case companion

Audio playing on iPhone.

case local

Audio playing on Apple Watch.

### Initializers

init?(rawValue: Int)

## Relationships

### Conforms To

- BitwiseCopyable
- Equatable
- Hashable
- RawRepresentable
- Sendable

## See Also

### SwiftUI

init(origin: WKInterfaceVolumeControl.Origin)

Creates a volume control for use in SwiftUI.

