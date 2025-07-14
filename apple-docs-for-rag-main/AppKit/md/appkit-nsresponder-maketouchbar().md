

- AppKit
- NSResponder
-  makeTouchBar() 

Instance Method

# makeTouchBar()

Your custom subclass of the `NSResponder` class should override this method to create and configure your subclass’s default NSTouchBar object.

macOS 10.12.2+

``` source
@MainActor
func makeTouchBar() -> NSTouchBar?
```

## See Also

### Supporting the Touch Bar

var touchBar: NSTouchBar?

The NSTouchBar object associated with the responder.

