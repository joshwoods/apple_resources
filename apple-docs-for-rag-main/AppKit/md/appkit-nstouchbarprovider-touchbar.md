

- AppKit
- NSTouchBarProvider
-  touchBar 

Instance Property

# touchBar

The property you implement to provide a Touch Bar object.

iOS 13.0+iPadOS 13.0+Mac Catalyst 13.1+macOS 10.12.2+

``` source
@MainActor
var touchBar: NSTouchBar? { get }
```

**Required**

## Discussion

This property supports key-value observing, which is used by the system, for example, if you replace a running bar. Many subclasses of NSResponder implement this property and conform to the NSTouchBarProvider protocol.

