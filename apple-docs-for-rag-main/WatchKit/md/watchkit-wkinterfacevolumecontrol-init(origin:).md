

- WatchKit
- WKInterfaceVolumeControl
-  init(origin:) 

Initializer

# init(origin:)

Creates a volume control for use in SwiftUI.

watchOS 6.0+

``` source
init(origin: WKInterfaceVolumeControl.Origin)
```

## Parameters 

`origin`  

The source of the audio managed by the volume control. For a list of possible values, see WKInterfaceVolumeControl.Origin.

## Discussion

Use this initializer to create an instance that you can wrap in a WKInterfaceObjectRepresentable view. If you aren’t using SwiftUI, create the control by dragging it from the Object library to your storyboard instead.

## See Also

### SwiftUI

enum Origin

The source of the audio managed by the volume control.

