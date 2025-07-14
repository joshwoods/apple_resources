

- AppKit
- NSResponder
-  touchBar 

Instance Property

# touchBar

The NSTouchBar object associated with the responder.

macOS 10.12.2+

``` source
@MainActor
var touchBar: NSTouchBar? { get set }
```

## Discussion

If you have not explicitly provided an NSTouchBar object for a responder by setting this property, the system sends the makeTouchBar() message to the responder to create the default bar. This property is archived.

## See Also

### Supporting the Touch Bar

func makeTouchBar() -> NSTouchBar?

Your custom subclass of the `NSResponder` class should override this method to create and configure your subclass’s default NSTouchBar object.

