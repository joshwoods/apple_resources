

- Playground Support
- PlaygroundPage
-  liveView 

Instance Property

# liveView

A live view that shows the result of running the code that’s on the current page.

macOS 11.0+Xcode 10.2+Swift Playgrounds 2.0+

**macOS**

``` source
final var liveView: (any PlaygroundLiveViewable)? { get set }
```

**Swift Playgrounds**

``` source
var liveView: PlaygroundLiveViewable? { get set }
```

## Discussion

Display a live view by setting `liveView` to an object that conforms to the PlaygroundLiveViewable protocol. Dismiss any open live view by setting `liveView` to `nil`.

The live view is displayed in the assistant editor for the current playground page. There can be only one live view open at any time.

Displaying the live view requires that needsIndefiniteExecution be set to `true`. When `liveView` is set to a non-`nil` value, the system sets needsIndefiniteExecution to `true`.

## See Also

### Configuring Live Views

static let current: PlaygroundPage

The current playground page.

func setLiveView&lt;IncomingView>(IncomingView)

Displays a SwiftUI view that shows the result of running the code that’s on the current page.

func setLiveView&lt;IncomingView>(IncomingView)

Displays a view that shows the result of running the code that’s on the current page.

