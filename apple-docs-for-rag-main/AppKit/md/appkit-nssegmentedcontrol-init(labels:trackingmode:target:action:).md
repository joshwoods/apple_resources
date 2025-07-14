

- AppKit
- NSSegmentedControl
-  init(labels:trackingMode:target:action:) 

Initializer

# init(labels:trackingMode:target:action:)

macOS 10.12+

``` source
@MainActor
convenience init(
    labels: [String],
    trackingMode: NSSegmentedControl.SwitchTracking,
    target: Any?,
    action: Selector?
)
```

## See Also

### Creating a Segmented Control

convenience init(images: [NSImage], trackingMode: NSSegmentedControl.SwitchTracking, target: Any?, action: Selector?)

