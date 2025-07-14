

- UIKit
- UIResponder
-  touchBar 

Instance Property

# touchBar

The Touch Bar object for the responder.

Mac Catalyst 13.0+

``` source
@MainActor
var touchBar: NSTouchBar? { get set }
```

## Discussion

This property’s default value — on devices with a Touch Bar — is the NSTouchBar instance that the responder’s makeTouchBar() method returns. Otherwise, the default value is `nil`.

## See Also

### Managing the Touch Bar

func makeTouchBar() -> NSTouchBar?

Asks the receiving responder to create and configure a Touch Bar object.

